# 2. การติดตั้งโปรแกรมและทดสอบตัวบอร์ด

โปรแกรมสำหรับเริ่มต้นใช้งานโกโกบอร์ดนั้นคือ GoGo Widget จำเป็นต้องมี Google Chrome เพื่อติดตั้งโปรแกรมดังต่อไปนี้ โดยคลิกที่ลิงค์ด้านล่าง

[![](https://lh3.googleusercontent.com/9eEJ90mosH6R_LXYh5jNVyqh1zzyiXkOmM6vEeovnTOP3Sw_kamFYiTNHibqkgXh3TkXDJKNItBtAMaDQtwGLexWuKLugEoknBKnAXeizbu-lswaQIOCINkPNd-jAggg5AKpeQFH)](https://chrome.google.com/webstore/detail/gogo-widget/onipnjeomppihdnpnhkffennhafpbkcg)

[คลิกเพื่อติดตั้ง GoGo Widget จาก Chrome Web Store](https://chrome.google.com/webstore/detail/gogo-widget/onipnjeomppihdnpnhkffennhafpbkcg)

{% hint style="info" %}
การใช้งานโกโกบอร์ด สามารถใช้งานได้ทันทีเมื่อเสียบเข้ากับคอมพิวเตอร์ ไม่จำเป็นต้องลง Driver ใดๆ เนื่องจากตัวบอร์ดมีการทำงานเช่นเดียวกับเมาส์หรือคีย์บอร์ด \(ใช้โปรโตคอลที่เรียกว่า HID\)
{% endhint %}

การทดสอบว่าตัวบอร์ดมีการทำงานตามปกติ ทำได้โดย อันดับแรกเชื่อมตัวบอร์ดเข้ากับคอมพิวเตอร์ด้วยสาย micro-USB ตรวจสอบให้แน่ใจว่าเลื่อนสวิทซ์ On/Offไป ที่ตำแหน่งเปิด \(On\) เมื่อบอร์ดเริ่มทำงานท่านจะได้ยินเสียง "**ปี๊บ ปี๊บ**" และหน้าจอแสดงผลบนบอร์ดจะแสดงคำว่า "**GoGo**" เป็นเวลา 1-2 วินาที รวมไปถึงโปรแกรม GoGo Widget บนคอมพิวเตอร์จะแสดงรูปภาพของตัวบอร์ดนั้นด้วย เป็นการบ่งชี้ว่าตัวบอร์ดยังทำงานตามปกติ

![](https://lh5.googleusercontent.com/szzE5WytiguqHDN6-DMTn_SQtPbfIzLblmifgCWWu_0FL_aP38MW6tN9GzZZL84yB5Ls2fH9XsY_7JNy4tg_8vcNiywvZGlOSp64u6d9EPFdKzBzExILVWGpiaDcgj5Q9e7sT51l)

รูปภาพข้างต้นที่ตัวโปรแกรมแสดง**เครื่องหมายคำถาม** แปลว่าไม่มีตัวบอร์ดเชื่อมต่ออยู่

![](https://lh4.googleusercontent.com/Mxys-VQMLJqW6mBLcSebEakfLMHW002dg4DMhHJZ5xW_sSUbpOYpeFMp2caEWUuWPB6DkIQ-Npwx195sJOk_di0SAMXh6LhkTpureebBtgsZetDWBK6pKgxkWJuz-twfmKaIN6kJ)

เมื่อเชื่อมตัวบอร์ดสำเร็จจะแสดงรูปภาพตัวบอร์ดดังข้างบน ซึ่งเป็นสิ่งที่เกิดขึ้นตามปกติเพียงแค่ต่อสาย USB จากตัวบอร์ดเข้ากับคอมพิวเตอร์และเลื่อนสวิทช์เพื่อเปิดบอร์ด

ขั้นตอนที่ง่ายที่สุดต่อจากนี้คือการสั่งให้ตัวบอร์ดส่งเสียง "ปี๊บ" และควบคุมไฟ LED บนบอร์ดโดยไอคอนที่ใช้ควบคุมคำสั่งเหล่านี้จะอยู่ด้านขวา ของตัวโปรแกรม ซึ่งมีคำสั่งต่างๆดังนี้

| **ไอคอน** | **คำสั่ง** |
| :---: | :--- |
| ![](https://lh6.googleusercontent.com/8FmSql-_1P0nCO4_9UsIdHhhRCYYXJWJqCyNW9MDAlf9FP-O_CWxEcXb4jwxR-ZN8D-UYBRt6ctni1hKtgWknTraLmtia2gfR_IH2M1YgGHYS9Q3cMKjs7QfB-87TWTr5reEgzBy) | **BEEP** - เมื่อเรียกใช้งานจะไปยินเสียง "ปิ้บ" จากตัวบอร์ดซึ่งเป็นการยืนยันว่าบอร์ดยังทำงานตามปกติ |
| ![](https://lh6.googleusercontent.com/zx-wsh643kjo_i74GhX90anuzRghTUiG4YliWFlQ4chAad4bb1oTft8o_7f79996N11caKmbwr1hvFZlNN2_1pogzxI0fXDV6iDO9eenUW1soUNuBTDJtLENi_-wc3VrPXnef1mw) | **LED ON** - สั่งเปิดไฟ User LED \(อยู่ที่ตำแหน่งมุมล่างขวา\) |
| ![](https://lh6.googleusercontent.com/DfOtLAzvJho0LlYCKXhKqi7t2fcuD4ub9oTqDhQ2Lk5E4Y5ZA5esTOYFV20m1kUhNmyHbsnv10jFdVF219GGJOMMbr4Y-ZuzkvHzBqAFMGQKknZN8Vb4yxWvyilf-flS8UmjTxpq) | **LED OFF** - สั่งปิดไฟ User LED |



