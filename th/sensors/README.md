# 3. การใช้เซนเซอร์

โกโกบอร์ดสามารต่อกับเซนเซอร์แบบอนาลอกได้ทั้งหมด 8 ตัว โดยพอร์ทสำหรับเสียบเซนเซอร์นั้นจะเรียงกันอยู่ที่ด้านล่างของตัวบอร์ดโดยมีการระบุลำดับของเซนเซอร์กำกับไว้ นอกจากนั้นตัวบอร์ดสามารถต่อกับเซนเซอร์ดิจิตอลได้อีก 2 พอร์ท ตำแหน่งของพอร์ทสำหรับเซนเซอร์ดิจิตอลจะอยู่ตรงมุมด้านขวาบนของตัวบอร์ดและมีการระบุ I2C-1 และ I2C-2 กำกับไว้เช่นกัน

ในชุดโกโกบอร์ดจะมาพร้อมกับชุดเซนเซอร์แบบอนาลอกหลายหลายชนิด ซึ่งเซนเซอร์ชนิดนี้ใช้งานได้ไม่ยาก โดยแบบพอร์ทที่ใช้ต่อเซนเซอร์เข้ากับบอร์ดถูกออกแบบมาให้ใช้เป็นมาตรฐานที่เรียนกว่า “[Grove](http://www.seeedstudio.com/wiki/Grove_System)” ซึ่งเป็นมาตรฐานของสายสำหรับต่อกับเซนเซอร์และตัวขับต่างๆ สารมารถดูเซนเซอร์ทั้งหมดที่ใช้มาตรฐานนี้ได้ที่ [SEEED studio](https://www.seeedstudio.com)

> Cation เซนเซอร์จาก SEEED store อาจจะใช้ร่วมกับโกโกบอร์ดไม่ได้ ให้ท่านตรวจสอบความเข้ากันได้ของเซนเซอร์ก่อนทำการสั่งซื้อ

การใช้เซนเซอร์นั้นไม่ยากเพียงเสียบสายเข้ากับตัวเซนเซอร์ และอีกด้านของสายเสียบเข้ากับพอร์ทเซนเซอร์บนบอร์ด บนตัวโปรแกรม GoGo Widget จะแสดงค่าของเซนเซอร์แต่ละพอร์ทโดยอัตโนมัติโดยจะแสดงออกมาในรูปแบบของกราฟแท่งพร้อมกับค่าของเซนเซอร์กำกับอยู่

ดังตัวอย่างข้างล่างนี้ เป็นการต่อเซนเซอร์แสงเข้ากับพอร์ทเซนเซอร์ 1 จะเห็นได้ว่าค่าเซนเซอร์นั้นมีการเปลี่ยนแปลงซึ่งเกิดจากระดับความเข้มของแสงที่แตกต่างกัน หากใช้มือบังแล้วจากนั้นค่อยปล่อยมือออก ค่าของเซนเซนเซอร์ 1 ก็จะเปลี่ยนแปลงด้วย

![](https://lh6.googleusercontent.com/6yTco31szs6078l93HRB9q2I76E3GgGeaKNruVVN66T6WFMgW_M0cGlpu2hOnONOXDoEWIIZLyXZ5Y3jreHbETzOVykryOB-cv_hnki3Je2jrOPeu8WFrVxAcG9uMgyK0n3-mQMf)![](https://lh3.googleusercontent.com/5dL8I6zWLLvC7u3JPIC1LAeM7tLWCnavBtvvwpu-FAdT0WEqNpzUaqozXyUVSACS5wAN1S17FMF1iOWgyrghnHvCchIhDD5QQxd7zyvvWF73oxubuNA5S8d7K1UkaaQaQpXTa5bt)

![](https://lh5.googleusercontent.com/QvWqZgmP5hgKislAgSgjRPdADaLEkf2cjYgF2TIwoosQU1xMpPBqeaMQ7W3Mko0_N3bL6B9fZQcymhigVojpzzdaIbazg0wFjREoCyLNZz_dTVztJNF00lO5ZOZdT_DFuRHytgri)![](https://lh3.googleusercontent.com/vacLSnU69A5KbTvpA-7kqdfsQ_ljvbpEYNq7-fAAe5LVwR9Z7kq2YY8nTq4PZU3tMXivyzBnZB0ymlh5MZEde96ERP4jpwD_FOSQXCLpisdlz_56eq-tsVyLOlV0rTRq_L4ZfrIR)

ค่าของเซนเซอร์จะสูงดังรูปข้างบน เนื่องจากได้รับแสงมากกว่ารูปข้างล่าง

