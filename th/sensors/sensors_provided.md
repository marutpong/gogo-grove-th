# 3.1 เซนเซอร์ที่มากับชุดโกโกบอร์ด

## **ลิมิตสวิทช์และปุ่มกด**

![](https://lh6.googleusercontent.com/XXhoiviM0cP9LWZSgzPx0pWmHF0x-tR4V8OhTWUseZfxY3xGaHsyGhh-O5gTvfPI-BFfGeMEibbzyN9AMxTOgTI_vG4uYLYIu8t6anoM7GqdF8GhQbq1BX0YVVc38N52Md8o0loC)

ลิมิตสวิทช์และปุ่มกดนั้นมีการทำงานที่คล้ายกัน ทั้งคู่มีค่าเซนเซอร์สูงเมื่อกด และมีค่าเป็น 0 หรือใกล์เคียงเมื่อปล่อย **ลิมิตสวิทช์** เหมาะสำหรับการตรวจจับวัตถุอย่างเช่น ผนัง ลูกบอล และกลไกต่างๆ ส่วน**ปุ่ม**นั้นเหมาะสำหรับให้ผู้ใช้กด

## **ชุดปุ่มกด** {#button-set}

![](https://lh5.googleusercontent.com/VUuiVQfDIceaurA8ryCCKjCOdan_ojwqc-Ogk9oiTRG6wBkPoh3-9_3EjxNkxEgRUqDUo_AL_sG_9mdyHAXpLfrVwb0iCmKGt-oUY4JY7gBwwPLyMTdp5RJ7jfbck4nPfMl6uJOx)

**ชุดปุ่มกด**มีประโยชน์เมื่อหากต้องการใช้ปุ่มหลายปุ่มโดยใช้เซ็นเซอร์เพียงพอร์ทเดียว การใช้ประโยชน์อย่างเช่น ทำเป็นตัวควมคุมเกมส์ หรือควบคุมการเคลื่อนที่ต่างๆ โดยเมื่อกดที่แต่ละปุ่มจะให้ค่าเซนเซอร์ที่ต่างกันออกมา

## **เซ็นเซอร์แสง** {#light-sensor}

![](https://lh5.googleusercontent.com/Rmta4SQ9rb1CuqJC9vY8uw2z4zgpFS7AN6q9hSuqbtxWINkbDGAognrPA6hnccv69Y8ekl-TX3fxjedsuwo3xmHmx09xpjsnYAJB_OJgzHxJvoyNSvG8lybrCexIjteQXqjVuOnZ)

**เซ็นเซอร์แสง** จะแสดงค่าต่างๆ ตามความเข้มของแสงที่ตัวเซ็นเซอร์ได้รับ

## **เซ็นเซอร์อุณหภูมิแบบอนาล็อก** {#temperature-sensor}

![sensor temperature.png](https://lh4.googleusercontent.com/GgtVOBlhdmGlF5LMSz3Avz-HLId9joXpfCZim2qFtt0QcdBQ25VHQd26BjgpoJD-vrjQtmdlnh5DhBlurrMIGVKLwScvIS4_8jwphbhye3EXrXdJP_gFW9FFYLhtqAdA9J5Dwn5j)

**เซ็นเซอร์อุณหภูมิ จะแสดงค่าแปรผันตามอุณภูมิที่เซนเซอร์ตรวจจับ**

> หน่วยของเซนเซอร์ไม่ใช้ องศาเซลเซียสหรือฟาเรนไฮต์ หากจะใช้วัดในหน่วยดังกล่าวจะต้องเทียบค่าจากเซนเซอร์และค่าอุณหภูมิในหน่วยนั้นๆ

## **เซ็นเซอร์แม่เหล็ก** {#magnetic-sensor}

![](https://lh6.googleusercontent.com/CQGNhkdfH75drhz385lKoW1OglalqJBSMLQhiySijjqP--X6O6tu1wlXJOunjBo812kH5iarjZ3BdrSkZTjiJ4qFYrz-Be1pFbg5Ih_bgaO-koYnUkgcByjTe5c2BLh3POmkZuE5)

**เซ็นเซอร์แม่เหล็ก** จะวัดค่าความเข้มของสนามแม่เหล็ก มักใช้กับการตรวจจับที่ไม่ต้องมีการสัมผัส เช่นวัดความเร็วของล้อจักรยาน โดยติดตำแหน่งเซ็นเซอร์ไว้ที่เฟรมจักรยาน ส่วนแม่เหล็กติดไว้ที่ล้อเมื่อล้อมีการหมุนเคลื่อนที่ในแต่ละรอบ เซ็นเซอร์สามารถตรวจจับว่ามีแม่เหล็กเคลื่อนที่ผ่าน และเมื่อจับเวลาในแต่ละรอบก็สามารถนำมาคำนวณเป็นความเร็วของจักรยานได้

## Infrared Reflective Sensor {#infrared-reflective-sensor}

![](https://lh6.googleusercontent.com/9bqUi-qv_uhq71zSn1qe5G5Q2os-9ULuRJx4bYSiWGFkwLS6zst3X9RLamf2FFtss5Z84vbJSwBFot1EuPXAiKHHl78HWCK0QvImOj_90SzTNkjAKNDW9R7ATZbA-Ty3MOQCzG-f)

This sensor is commonly used to measure proximity. It emits infrared light and measures how much of that light is reflected back. Therefore, if there is no object to bounce back the light, the sensor will give a small measurement. The closer an object is to the sensor, the higher the measurement. The effective range of this sensor is less than 5 centimeters. Note that color of the object also determines how much light is reflected. For example, black objects absorbs more light than lighter colors and, at the same distance, produces a lower measurement. Therefore, this sensor can also be adapted as a color sensor.

> **Caution** - This sensor is sensitive to infrared light from other sources as well. Therefore, the interference of sunlight, fluorescent light or other infrared light sources may lead to irregular readings.

## **เซนเซอร์น้ำฝน** {#rain-sensor}

![sensor rain.png](https://lh6.googleusercontent.com/CfP5LQKjRSXzFGOnuqzSghzV4rAUu6DPD7DwLa5ZfnhmXN8CpqvpPtg5rDMCYnX90mYWqtnHv-SApJSrw7jd4kprxunTzj0wi4qAgi-3HP3QB5qRG6e1Uy38ju5tB-EuAfmII9am)

**เซ็นเซอร์น้ำฝน** จะมีโลหะที่อยู่ใต้เซนเซอร์ที่สามารถตรวจจับหยดน้ำฝนได้ ในการตรวจจับน้ำฝนหรือหยดน้ำควรให้โลหะดังกล่าวหงายขึ้น และตรวจสอบให้แน่ใจว่าส่วนที่เป็นสายไฟนั้นจะไม่โดนน้ำฝนด้วย

## **เซนเซอร์วัดความชื้นในดิน** ![](https://lh5.googleusercontent.com/ShjcJG_JzPDLen6CHoZZ4e0Sj32jGRE9LkxeuEOF3dj6xbNRnLBs99zIflF2-HfLuEQvP3Mxs25vxdhhigT3l7XoaJ09EYUyPRfVp_y9uOvdiCScQY8JnIfMLVQ_Ea48FmfoWtS4)

**เซนเซอร์วัดความชื้นในดิน**ประกอบด้วยโลหะ 2 แผ่น เมื่อปักต่อเซ็นเซอร์ลงในดินควรตรวจสอบให้แน่ใจว่าตัวขั้วโลหะหรือสายนั้นแห้งไม่สัมผัสกับดิน

## **ตัวแปลงสาย**

## ![](https://lh6.googleusercontent.com/BsDQ0Lmmj7k9reFACTEsyOA4DZzNWpNU4UPFLcLUXE90ZmSS-JHGJHknNh9i-nWG90HLG6i3DOGQdDADIxE3sIH4rUigGNeczo-xpQE5f32wpqlR7wWbCZlke0e652HwQEYGV5Og)

**ตัวแปลงสาย**นี้ใช้สำหรับแปลงเซนเซอร์ชนิดอื่นอื่นๆที่ไม่ได้อยู่ในชุดนี้ ให้ใช้ร่วมกับ**โกโกบอร์ด**ได้ โดยเชื่อมต่อกับไฟ กราวน์ และสายสัญญาณ เป็นขั้ว VCC, GND และ Sig ตามลำดับ

