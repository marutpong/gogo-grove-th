# 7.3 DC Motor Control

Connect a DC motor to port A and try the code below using either Logo or Tinker.

```text
to motorcontrol
    a, on wait 10 off 
    beep
end
```

![](https://lh5.googleusercontent.com/Jbk5hycO-WZuUA2C9HCJ5L7YL_Ydjp2rceHi2Hc1MkY_k6fTPnQhwT0IEZWGAbA7HTRYpBsWlmvcLqECfU2m07FYY5l247QnR-xzlAvpnQOMwTlg4fNCXuuIDKP37-icf1gjcJPp)

This program will turn on motor A for 1 second \(the wait command has a unit of one-tenth of a second\)

## Motor Selection {#motor-selection}

Before performing any action, a motor port or ports must first be selected. In Logo, this is done using the port name followed by a comma. For example, “a,” will select port A. “ab,” will select both port A and B. “abcd,” will select all four ports. Notice that the alphabetical order does not affect port selection. That is “abcd,” is the same as “dcab,”.

In Tinker, motor port selection is done visually using the “talk to motor” block. Tick on the port name to select that port. The example below will select port A.

![](https://lh5.googleusercontent.com/RIAlPz8CQ7XIGrdMehV3reiucfcil0c99liiPaG71Vr4kStlOZeAkXA-BfU0kNk9_ppYzzxuTptX7lCK0zso5N8_iPFtGKnW-F4nJfPyqAjz6Ut2UxIb7NkI8Bi0gMhrbI11In1W)

## Motor Actions {#motor-actions}

Once a port or ports have been selected, actions can be performed on them as shown below.

| Tinker | Logo | Action on the selected motor\(s\) |
| --- | --- | --- |
| ![](https://lh3.googleusercontent.com/82GjzdzOq9LYwsMe8EpSkSVeH6bfhBBpsKptv5Ux22OwqyodW5AvPnvhioqcEEeiJozItqjyAm401n54wt0Naz0fTmF4iIimVQWb5fwiXqNKlWTB7IuQNjOYnztrr5OIlgYAMpzL) | on | Turns on |
| ![](https://lh6.googleusercontent.com/mjbh4vLuagsuwlIVP2g7fzAIU88Yzbp3hNDmiDJE5SoqbjTASnYIVdo7dorB3RxRM9Su9SpNqVRofnh8Fgr3trR551Dezjow6zJ9VQEab5gkEu4zLv1LqrhU70HyXLuO7dNN_3g7) | off | Turns off |
| ![](https://lh4.googleusercontent.com/QhDfp0haE1-fOktFgiiEoYy5gG2hFHXsQ5MbQKsnEDtimY89_LdiRHx4b39LVJCgEGWCFWsyY03xSsaGj3VFM8vTrjRNi4r4PDuM5dbD0qekpDZ6AJDNyvbHmustBSdAZ1ywzeCy) | onfor 1 | Turns on for one-tenth of a second. This number can be changed. |
| ![](https://lh4.googleusercontent.com/NJ2Sw3t-iL8ToSnF-LYS1JzV9Z8r3l0gG2Ye3IL5jg320GU7h3UyGKvpUS_6X0kL_8nWhfajlNhgwmJGosQ2b9p7gLeF8Bk1S36HDFIEOc7pXKdDGvSjcsw1xJR5IZ-L3S3DXqvJ) | cc | Rotate motor clockwise |
| ![](https://lh4.googleusercontent.com/3sklhEVuJp2ymW_9vYY-kg0bJJiAC56lLltfkeUudTJvnmQOhHXcWC39gbjBIPMPTQ3q95zmkAj5pgkzYzi0j_x3CQOoACfHtBsMWbpth6phHKN8Qt_6ixl1t7f9d7nz8ZYRugty) | ccw | Rotate motor counter-clockwise |
| ![](https://lh6.googleusercontent.com/43etM4CC6PygS1UxvnV8s_zUpf2GOzX1Na3lRBGk2ue1yitfVWf0STQNDqWlUr7veCsk6TQoGYgy9_y2jIwI-g8ENwB8LrZPLvSwQ34H4d-KwKauvbb_k-kbtUTQlf0nIVX07MUe) | rd | Reverse the current rotation to the opposite direction. |
| ![](https://lh3.googleusercontent.com/rjYw9NvwIOvMNSt2NmFXyDMu_40AwlWihKARenoMk8Y8HOAHzTvy6o1TzfwpWP5tOGZVIbCm38nCpL_XyUUrNRDlcHcd8D0XHSXZw4u4pNz8nj6Ra2gOjh5v6zKUlkkg5v932uiY) | setpower 100 | Set the power level to 100. This number can be between 0 \(off\) to 100 \(full power\). |

## Motor State {#motor-state}

The on-off state of the motor ports can be tested using the following reporter.

| Tinker | Logo | Value |
| --- | --- | --- |
| ![](https://lh3.googleusercontent.com/2Pnfjx3dr7Rm_r2M7G-dxoBgX0OJlbw8QvF6OvD910mJ4YcUkbI6sKZmsgThrLJAOXZfhAO4-cu87AZRs7QFMDR368pcYLWKv06xF4UhqpTqjygwTvTfogaMG8EIoox76H9nGMMO) | aon? | Returns “true” if the specified motor is “on”. If more than one port is selected, returns “true” only if all ports are on. |

Here’s an example that will turn off port A if it is on.

```text
to off_if_on 
    if aon? [ a, off] 
end
```

![](https://lh5.googleusercontent.com/TDpKihyV6sk349K6SoFBkFG2iBiJZY8_BC9odY2JeoUg_aHxwQ1oTcvo1dl6MzTvX7HJuTt7Zc70jTEtSGOxcQLJco1onvd5An44C2UjueXbRUjRuwQQle8eSAnGtmXihoL-AE8l)

