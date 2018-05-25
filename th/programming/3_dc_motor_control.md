# 7.3 การใช้งานมอเตอร์กระแสตรง \(DC Motor\)

เชื่อมต่อมอเตอร์เข้ากับพอร์ต A แล้วทดลองใช้งานโปรแกรมด้านล่างโดยใช้ภาษาโลโก หรือ Tinker

```text
to motorcontrol
    a, on wait 10 off 
    beep
end
```

![](https://lh5.googleusercontent.com/Jbk5hycO-WZuUA2C9HCJ5L7YL_Ydjp2rceHi2Hc1MkY_k6fTPnQhwT0IEZWGAbA7HTRYpBsWlmvcLqECfU2m07FYY5l247QnR-xzlAvpnQOMwTlg4fNCXuuIDKP37-icf1gjcJPp)

โปรแกรมนี้จะสั่งมอเตอร์ A ให้ทำงานเป็นเวลา 1 วินาที \(คำสั่ง wait มีหน่วยเป็น 1/10 วินาที\)

## การเลือกพอร์ตมอเตอร์ {#motor-selection}

ก่อนที่จะใช้งานใดๆ จำเป็นจะต้องเลือกพอร์ตมอเตอร์ที่จะใช้งานก่อน ในภาษาโลโก้ทำได้โดยระบุชื่อพอร์ตมอเตอร์ที่จะใช้แล้วตามด้วยคอมม่า ตัวอย่างเช่น "a," จะเป็นการเลือกใช้งานมอเตอร์พอร์ต A "ab," จะเป็นการเลือกใช้งานมอเตอร์ทั้งพอร์ต A และ B "abcd," จะเป็นการเลือกใช้งานมอเตอร์ทั้ง 4 พอร์ต

> **ข้อสังเกต** ลำดับของตัวอักษรจะไม่มีผลกับการเลือกใช้งานพอร์ตมอเตอร์ การเลือกใช้งาน "abcd," จะให้ผลลัพธ์เหมือน "dcba,"

ใน Tinker การเลือกสั่งงานพอร์ตมอเตอร์สามารถใช้งานผ่านบล็อก "talk to motor" ติ้กเลือกพอร์ตตามชื่อพอร์ตที่แสดงอยู่ในบล็อก โดยในตัวอย่างด้านล่างเป็นการเลือกสั่งงานพอร์ตมอเตอร์ A

![](https://lh5.googleusercontent.com/RIAlPz8CQ7XIGrdMehV3reiucfcil0c99liiPaG71Vr4kStlOZeAkXA-BfU0kNk9_ppYzzxuTptX7lCK0zso5N8_iPFtGKnW-F4nJfPyqAjz6Ut2UxIb7NkI8Bi0gMhrbI11In1W)

## การสั่งงานมอเตอร์ {#motor-actions}

เมื่อได้เลือกพอร์ตมอเตอร์ใดมอเตอร์หนึ่ง สามารถที่จะสั่งงานได้ดั่งที่แสดงในตารางด้านล่าง

| Tinker | **ภาษาโลโก้** | **ผลลัพธ์ของพอร์ตมอเตอร์ที่เลือก** |
| --- | --- | --- |
| ![](https://lh3.googleusercontent.com/82GjzdzOq9LYwsMe8EpSkSVeH6bfhBBpsKptv5Ux22OwqyodW5AvPnvhioqcEEeiJozItqjyAm401n54wt0Naz0fTmF4iIimVQWb5fwiXqNKlWTB7IuQNjOYnztrr5OIlgYAMpzL) | on | เปิดมอเตอร์ |
| ![](https://lh6.googleusercontent.com/mjbh4vLuagsuwlIVP2g7fzAIU88Yzbp3hNDmiDJE5SoqbjTASnYIVdo7dorB3RxRM9Su9SpNqVRofnh8Fgr3trR551Dezjow6zJ9VQEab5gkEu4zLv1LqrhU70HyXLuO7dNN_3g7) | off | ปิดมอเตอร์ |
| ![](https://lh4.googleusercontent.com/QhDfp0haE1-fOktFgiiEoYy5gG2hFHXsQ5MbQKsnEDtimY89_LdiRHx4b39LVJCgEGWCFWsyY03xSsaGj3VFM8vTrjRNi4r4PDuM5dbD0qekpDZ6AJDNyvbHmustBSdAZ1ywzeCy) | onfor 1 | เปิดมอเตอร์เป็นเวลา 1 ใน 10 วินาที โดยสามารถปรับเปลี่ยนเวลาได้ |
| ![](https://lh4.googleusercontent.com/NJ2Sw3t-iL8ToSnF-LYS1JzV9Z8r3l0gG2Ye3IL5jg320GU7h3UyGKvpUS_6X0kL_8nWhfajlNhgwmJGosQ2b9p7gLeF8Bk1S36HDFIEOc7pXKdDGvSjcsw1xJR5IZ-L3S3DXqvJ) | cc | สั่งให้มอเตอร์หมุนตามเข็มนาฬิกา |
| ![](https://lh4.googleusercontent.com/3sklhEVuJp2ymW_9vYY-kg0bJJiAC56lLltfkeUudTJvnmQOhHXcWC39gbjBIPMPTQ3q95zmkAj5pgkzYzi0j_x3CQOoACfHtBsMWbpth6phHKN8Qt_6ixl1t7f9d7nz8ZYRugty) | ccw | สั่งให้มอเตอร์หมุนทวนเข็มนาฬิกา |
| ![](https://lh6.googleusercontent.com/43etM4CC6PygS1UxvnV8s_zUpf2GOzX1Na3lRBGk2ue1yitfVWf0STQNDqWlUr7veCsk6TQoGYgy9_y2jIwI-g8ENwB8LrZPLvSwQ34H4d-KwKauvbb_k-kbtUTQlf0nIVX07MUe) | rd | สั่งให้มอเตอร์สลับทิศทางตรงกันข้ามกับที่หมุนอยู่ |
| ![](https://lh3.googleusercontent.com/rjYw9NvwIOvMNSt2NmFXyDMu_40AwlWihKARenoMk8Y8HOAHzTvy6o1TzfwpWP5tOGZVIbCm38nCpL_XyUUrNRDlcHcd8D0XHSXZw4u4pNz8nj6Ra2gOjh5v6zKUlkkg5v932uiY) | setpower 100 | ตั้งค่าให้มอเตอร์ทำงานเป็นระดับ โดยสามารถตั้งได้ระหว่าง 0\(ปิด\) - 100\(เร็วสุด\) |

## สถานะของมอเตอร์ {#motor-state}

สถานะของมอเตอร์สามารถที่จะทดสอบได้โดยใช้คำสั่งต่อไปนี้

| Tinker | **ภาษาโลโก้** | **ผลลัพธ์** |
| :--- | :--- | :--- |
| ![](https://lh3.googleusercontent.com/2Pnfjx3dr7Rm_r2M7G-dxoBgX0OJlbw8QvF6OvD910mJ4YcUkbI6sKZmsgThrLJAOXZfhAO4-cu87AZRs7QFMDR368pcYLWKv06xF4UhqpTqjygwTvTfogaMG8EIoox76H9nGMMO) | aon? | จะให้ค่าเป็น**จริง** เมื่อพอร์ตมอเตอร์ที่เลือกเปิดทำงานอยู่ ถ้าเลือกพอร์ตมอเตอร์มาก  กว่าหนึ่งพอร์ต จะให้ค่าเป็น**จริง** เมื่อทุก      พอร์ตที่เลือกเปิดทำงานอยู่ |

ตัวอย่างนี้แสดงให้เห็นว่า จะทำการปิดพอร์ต A ถ้าพอร์ต A เปิดอยู่

```text
to off_if_on 
    if aon? [ a, off] 
end
```

![](https://lh5.googleusercontent.com/TDpKihyV6sk349K6SoFBkFG2iBiJZY8_BC9odY2JeoUg_aHxwQ1oTcvo1dl6MzTvX7HJuTt7Zc70jTEtSGOxcQLJco1onvd5An44C2UjueXbRUjRuwQQle8eSAnGtmXihoL-AE8l)

