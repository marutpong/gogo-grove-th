# 7.7 การใช้งานตัวแปร

ตัวแปรเป็นเครื่องมืออย่างหนึ่งที่ทำให้โปรแกรมสามารถนับ เก็บข้อมูล กำหนดค่า และอื่นๆ ดังตัวอย่างต่อไปนี้ที่แสดงให้เห็นว่าตัวแปรถูกใช้สำหรับนับจำนวนครั้งการกดสวิตซ์และแสดงผลบนจอของโกโกบอร์ด โดยเชื่อมต่อสวิตซ์ที่พอร์ตเซ็นเซอร์ 1 และรันโปรแกรมต่อไปนี้

{% tabs %}
{% tab title="Logo" %}
```text
to press_count
    set counter 0
    forever [
        if sensor1 > 500 [ 
            set counter counter + 1 
            show counter 
            waituntil [sensor1 < 500]
        ]
    ]
end
```
{% endtab %}

{% tab title="Tinker" %}
![](https://lh6.googleusercontent.com/YIcKKPd6BdOsRpyhiBmMULTE1wGTkAPrzFzVu0PwLzO2FmxM390GV1zfk6d9Y0WIgp1UI10WL6AZ0KgDUuwC-yiu1cZ6YIk-h0Z2yUOYrWWILc1sBrV_z8AejLNQ2iYshJgdFvjy)
{% endtab %}
{% endtabs %}

คำสั่ง "set" ถูกใช้เพื่อกำหนดค่าในตัวแปร ในตัวอย่างข้างต้นโปรแกรมเริ่มต้นจากตั้งค่าตัวแปรชื่อ "counter" ให้มีค่าเท่ากับ 0 สังเกตว่าการตั้งค่าเริ่มต้นนี้ควรตั้งชื่อตัวแปรให้ถูกต้องเพราะจะนำไปใช้งานในส่วนที่เหลือของโปรแกรม ในตัวอย่างตัวแปรที่ชื่อ "counter" สามารถใช้เป็นอาร์กิวเมนต์สำหรับคำสั่งใดๆที่มีการรับค่า

{% hint style="info" %}
ใน Tinker ตัวแปรจะถูกระบุไว้ในส่วน “Variables” และสามารถจัดการได้จากตรงนั้น หากต้องการสร้างตัวแปรใหม่ ให้ลากบล็อก “set” ไปยังพื้นที่สำหรับเขียนโปรแกรม จากนั้นคลิกปุ่มเลือกแบบเลื่อนลง \(drop-drown\) จะมีรายการแสดงให้เลือก เพื่อเปลี่ยนชื่อ หรือสร้างตัวแปรใหม่
{% endhint %}

![](https://lh3.googleusercontent.com/5at4y_DcVZyn-h1WJaH5GqmF5772E-W9qP6dY01BqZDlH7DH6GXHfvr8qRZ0Xc8t75S6OckO79i0BGjO-qSpvwxujLyUm1KEMc-8bQvx7G45NJlBWzfy01dne1PgFViZoUmuWVk7)

