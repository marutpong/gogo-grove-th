# 7.8 การใช้งานรีโมทคอนโทรล

โกโกบอร์ดสามารถใช้งานร่วมกับรีโมทคอนโทรลได้ โดยใช้คำสั่งภาษาโลโก้ "**newir?"** และ "**ir**_"_ ดังตัวอย่างต่อไปนี้  


{% tabs %}
{% tab title="Logo" %}
```text
to ir_control
    forever [
        if newir? [
            set command ir 
            if command = 128 [ beep ]
            if command = 129 [ a, on ]
            if command = 130 [ a, off ]
        ]
    ]
end
```
{% endtab %}

{% tab title="Tinker" %}
![](https://lh3.googleusercontent.com/ycK3PlXra_KaA2enpLy_sAIAqGpjkf380wX7fMAaUF38Gy0RBqSmtmBk-nBHDrThuNE8YsbcVYlxr8_IsykvoeEjEUoPiPoTB-IG45yFEOWXjoieka4dW565mjS9T0-RnPUbPS2s)
{% endtab %}
{% endtabs %}

จากโปรแกรมตัวอย่างมีการเช็คเงื่อนไขว่า _มีคำสั่งจากรีโมทคอนโทรลหรือไม่_ ซึ่งใช้คำสั่งภาษาโลโก้ "**newir?**" หรือบล็อกคำสั่ง "**new infrared?**" เมื่อเป็นจริง ให้รับรหัสอินฟราเรด ใช้คำสั่งภาษาโลโก้ "**ir**" หรือบล็อกคำสั่ง "**get infrared**" โดยนำรหัสอินฟราเรดเก็บไว้ในตัวแปรที่ชื่อ **command** จากเงื่อนไขตามลำดับในตัวอย่าง มีการตรวจสอบรหัสอินฟราเรดที่รับมา แล้วสั่งทำงานตามแต่ละเงื่อนไข

