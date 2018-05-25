# 7.5 Program Control

The following example demonstrates a common use of program controls. Connect a button or switch to sensor 1 and a DC motor to the output port A. Then, try the following script.

```text
to sensor_control
    forever [
        if sensor1 > 500 [ a, on wait 10 off]
    ]
end
```

![](https://lh3.googleusercontent.com/RX7aD-7XjLrC8fdN2COk1b3qmD_DxJBKVE26B7X_PNge5djXd7xR8R53uSJqdf1Lq2UVKVbL5Oc2_NbLY7utTb8F-ITUL1Hz72ht_O2saeLgxB5dJFleC0XGZvwppfyG2O_uIL1j)

## IF {#if}

The IF program-control allows parts of the program to run only when the given condition is met. An IF is always followed by a condition. The example above shows an IF followed by a condition which reads “if sensor 1 is greater than 500”. Then, the commands to be executed are located in the “do” section. In this case, the program will turn on motor A for one second.

## Conditions {#conditions}

Defining a suitable condition for an IF is important. When using sensors, the first step is usually to observe how the sensor values change. Then a condition can be defined. In this example, the sensor value for an unpressed switch is usually 0. This value jumps to 1023 when the switch is pressed. Therefore, the condition “if sensor 1 is greater than 500” really means “if switch pressed”. The number 500 was selected as a rough mid-point between the highest and lowest possible values. Changing this threshold to other numbers such as 100 or 1000 will still work for this example.

Condition values are more sensitive when using analog sensors, which values change in proportion to their measurements. Consider a light sensor that is used to control a lamp so that the lamp switches on when the house is dark. Let’s say the sensor value is zero when there is no light during the night and the value increases and reaches 800 during the day. What will be a good threshold for the program? 400? The answer is that it depends on how dark it should be before the lamp turns on. A value too low will make the lamp too slow. A value too high will cause the lamp to switch on prematurely. In practice, the programmer will have to obtain a suitable threshold value by observing the sensor value at the time when the lamp owner feels it is dark enough to switch it on. In this case, the condition determines the lamp’s “light sensitivity”.

Conditions can be combined to form a more complex definition. Logical operators are often used. The example below shows a condition that requires two buttons to be pressed in order to turn on a motor.

```text
if sensor1 > 500 and sensor2 > 500 [ a, on wait 10 off]
```

## IF-ELSE {#if-else}

The IF-ELSE program-control is an extension of an IF. In addition to defining what actions to perform when the condition is true, IF-ELSE can also define what to do when the condition is false. The following example modifies the original example so that it turns on the motor when the switch is pressed and off when the switch is released.

```text
ifelse sensor1 > 500 [a, on] [ a, off]
```

![](https://lh4.googleusercontent.com/ndPgTRI-wVLPlQpLtO_gxfEdrTUAIxfZN33giTVr3foZEGoUmaYb8wVVaVkYj9XK_7yUqZjCp3lb1IDJKGpuHW72nkQ2IJq74S6SUEbqrjgGOXibXuzw2wZDV7Ci_aTFKXHpJkP3)

## FOREVER {#forever}

The FOREVER program-control tells the program to loop indefinitely, executing the blocks it contains. Most programs will need this loop. The sensor\_control example is shown again below with and without FOREVER \(right and left images respectively\). Without a FOREVER, the program will check the condition once and quit, which is not the desired behavior. This is a common mistake of beginners.

| ![](https://lh4.googleusercontent.com/Q4EEgXDJnV9EkXZOEx4blecRAjVWdzUHasmo4ORgeasnBrJAlKoT1tM6nwaQq1jBbeZicOTt1vjQ4UOAVaaqu2-dVKjZUNQhmHBqvOoFiky3cOwnYrEj1PrvWh9HPdGw1hXV9xdK) | ![](https://lh4.googleusercontent.com/G1fTh-Pcqm_u7QmlbQfUQzH6BX_erENFgirNtwvjt3BjMNsOD6yItjnq39xAqRoch5q4eov8oXMZcohXFapTA94s2_7MI7ipSUWhXVjSuIldxizaz3qOslQHq-xf3ZuRk6L0nukT) |
| --- | --- |
| Without FOREVER | With FOREVER |

## WAITUNTIL {#waituntil}

The WAITUNTIL program-control allows the program to halt until the given condition is true. The example program below shows how WAITUNIL is used so that the program beeps once every time a switch is pressed

```text
forever [ if sensor1 > 500 [ beep waituntil [sensor1 < 500]]]
```

![](https://lh5.googleusercontent.com/9OVLhSr3SZwCb99-3Lni6eKH6U8mZVMdJJhLWiEdsZf6Bl0LqgQ9tOLJC7f86wpJZi1VG0VfCZaWRu0b4KBroGn-ageKqrVaJHUxgID3G-5T_LaeMNOPaAcyepcLxBeu2c1Sgb8f)

Note that without the WAITUNTIL, the program will beep repeatedly while the switch remains pressed.

