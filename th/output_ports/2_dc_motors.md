# 4.2 DC มอเตอร์ \(มอเตอร์ไฟฟ้ากระแสตรง\)

![](https://lh6.googleusercontent.com/vugFhp63tFP9Drkpz6paC5wnt1y5VRU5k7AJGdcsuFF92q6sgcAQXyDcYTdNHnbXwvXOxYJ2DqqBwFrGt1odN8yJgFiySY3uSaT0paGLHJfRX4mDr1jsTdNDt86gNIT-NwuadnPL)

ในขั้นตอนต่อจากนี้ สามารถลองใช้งาน มอเตอร์กระแสตรงได้ โดยการต่อมอเตอร์ดเข้ากับล้อที่มีอยู่เฉพาะชุดGoGo Kit และต่อหัวต่อสีขาวของมอเตอร์เข้ากับพอร์ต A ของ โกโกบอร์ด

## การเลือกใช้งาน {#selecting-active-ports}

![](https://lh6.googleusercontent.com/dT00YXdHJb1CeOLMLZNGGOwKxKCfIbYhvI9bkarpO85GXWoYEERJDD3ad1N87VHcGxi7c1AcLLxRPvnK3A-3vHFDTfThYuBhXlsxZ9lQfViNx2Wd_Oyd7j38UX3yTqmAfdtKr9JD)

ในการใช้งาน พอร์ตส่งออกหรือเอ้าพุตนั้น ขั้นแรก สามารถคลิกที่วงกลมที่มีชื่อพอร์ตกำกับอยู่คือ A , B, C, D ดังภาพด้านบน

* พอร์ตที่ถูกเลือกให้ใช้งาน ลูกศรรอบวงกลมจะมีสีเขียวหรือสีแดง ในที่นี้ พอร์ต A และ B นั้นอยู่ในสถานะถูกเลือกแล้ว
* “ลูกศร” นั้นจะปรากฏสีตามทิศทางที่มอเตอร์หมุน\(หรือขั้วทางไฟฟ้า\) โดยทั้งสองสีจะมีทิศทางหมุนตรงข้ามกัน ในที่นี้มอเตอร์ A และ B จะเกิดการหมุนคนละทิศทาง 
* โดยปกตินั้น การคลิกที่วงกลมดังกล่าวเป็นแค่การเลือกพอร์ตมอเตอร์เท่านั้น โดยจะยังไม่มีอะไรเกิดขึ้น ซึ่งสามารถเลือกได้ว่าต้องการให้มอเตอร์ทำงานอย่างไร โดยสามารถคลิกปุ่ม “on” หรือ “off”  ได้ในหน้าต่างโปรแกรม
* พอร์ตที่กำลัง “ทำงาน” อยู่นั้นจะมีพื้นหลังของวงกลมเป็นสีเหลือง ในที่นี้จะเห็นได้ว่าพอต์ต A และ D กำลังทำงานอยู่ ซึ่งการคลิกอีกครั้งคือการไม่เลือกพอร์ตนั้นอีกต่อไป แต่การทำงาน จะคงอยู่ในสถานะเดิมก่อนหน้าต่อไป
* ส่วนพอร์ตที่มีวงกลมสีเทานั้น แสดงว่ายังไม่ได้อยู่ในสถานะการทำงาน ซึ่งในที่นี้ พอร์ต C นั้นอยู่ในสถานะ “ไม่ทำงาน” แต่พอร์ต D ยังคงสถานะ “ทำงาน”
* ส่วนตัวเลข ที่อยู่ด้านใต้แต่ละพอร์ต คือพลังงานที่จะส่งออกไปให้กับพอร์ตนั้นๆ โดยทั่วไปพลังงานจะมีค่าที่ 100 ซึ่งสามารถปรับค่าได้ตามต้องการในสไลด์บาร์

## การควบคุมมอเตอร์

{\#dc-motor-operations}

### ตารางดังต่อไปนี้ แสดงคำอธิบายของการควบคุมมอเตอร์

| ไอคอน | คำสั่ง |
| :---: | :--- |
| ![](https://lh3.googleusercontent.com/IRB7JV4Tr0BS45-EC3mrm8V27KUXKGsxuQAOxdRQ8VQJZ1JJ7Hzgbsi3ysu7OtidxS-FQ9D1ZOIDKU4sm7cZ48BYHxNafX0b4bcfcBZuXLhMuMiRMAwqVQ3LJiKUwEjx5gFKzKRM) | \(ON\) ปุ่ม – สั่งให้มอเตอร์ที่ถูกเลือกทำงาน |
| ![](https://lh5.googleusercontent.com/StVVFL5pQNIl3p4c9Q7j9Qjough20wPZsHBuFMKCgzQatQ_A7i8XACa_iCOJv1wtxepKenfnPxl12oUasqQVUSnkt6CoAylQzWFGH94ywiOOWcsg9xKhSbqEeAmpevs9bNjiiWAV) | \(OFF\) ปุ่ม – สั่งให้มอเตอร์ที่ถูกเลือกหยุดทำงาน |
| ![](https://lh4.googleusercontent.com/pPOWCQOU2wZkvr-FeG5kLxV0YfxXpI0WGQaO-Lt9dJoQFRFJppisPxaZWEDoWW9La6bxkbpvqByFr4I-PPYFBUHGdwmvevujcfUxGZBC2_6qLz4BJ3QIFWEaKBJrdV8wUwyhVcud) | \(CCW\) ปุ่ม – ตั้งค่าทิศทางให้หมุนทิศทวนเข็มนาฬิกา \(counter clockwise\) |
| ![](https://lh3.googleusercontent.com/T81kVG8BQNbrXyjzLqbqtoX4k5qofblSREYOecOEOQ3hceVShJjubvC5jfT2IxFcpF0ObEkURqWI80OWC8EQvm-QR11yVlsuqbpizXfEUpOxB9PMFUm-kpqczcEvFCxxZ9dIdcBE) | \(RD\) ปุ่ม -  สั่งให้มอเตอร์หมุนตรงข้ามกับทิศที่หมุนก่อนหน้า \(reverse direction\) |
| ![](https://lh3.googleusercontent.com/8M5RDyhnOqeMWH1XsryqKRHlUA3a61DH7AvGVBCU0vIY6kpIUDQ-Rj2xRTG0-6jMbwnYqp4UYAaxpbKfg--RU8GZGsQqTYH_5ZrkVRBABglmp_O5Rx453hPIgWvY0x0eB2mvtSpu) | \(CW\) ปุ่ม - ตั้งค่าทิศทางให้หมุนทิศทเข็มนาฬิกา \(clockwise\) |

![](https://lh6.googleusercontent.com/-BUooz3wAnPl26pncYrMSS4p5Gz66H9iehoiytXGetB195k9kPuXjA1Ik2b-6aqq5Du34osabegEZ7rs3Q6ZuVviay1bY2aRB9asCEc6IAQWEmBI8l-KZfhNT6RtpVoeQkkmk5-k)

**การตั้งค่าพลังงาน** - สามารถเลื่อน ตัวเลื่อน ที่แสดงถึงค่าพลังงานที่จะใช้งาน และเมื่อที่ได้ค่าที่ต้องการให้กด “ตั้งค่าพลังงาน” \(Set Power\)

