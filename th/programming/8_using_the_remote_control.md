# 7.8 การใช้งานรีโมทคอนโทรล

โกโกบอร์ดสามารถใช้งานร่วมกับรีโมทคอนโทรล โดยใช้คำสั่งภาษาโลโก้ "_newir?"_ และ "_ir"_ ดังตัวอย่างต่อไปนี้

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

![](https://lh3.googleusercontent.com/ycK3PlXra_KaA2enpLy_sAIAqGpjkf380wX7fMAaUF38Gy0RBqSmtmBk-nBHDrThuNE8YsbcVYlxr8_IsykvoeEjEUoPiPoTB-IG45yFEOWXjoieka4dW565mjS9T0-RnPUbPS2s)

จากโปรแกรมตัวอย่างมีการเช็คเงื่อนไขว่า _มีคำสั่งจากรีโมทคอนโทรลหรือไม่_ ซึ่งใช้คำสั่งภาษาโลโก้ _"newir ?"_ หรือบล็อกคำสั่ง _"new infrared?"_ เมื่อเป็นจริง ให้รับรหัสอินฟราเรด ใช้คำสั่งภาษาโลโก้ _"ir"_ หรือบล็อกคำสั่ง _"get infrared"_ โดยนำรหัสอินฟราเรดเก็บไว้ในตัวแปรที่ชื่อ **command** จากเงื่อนไขตามลำดับในตัวอย่าง มีการตรวจสอบรหัสอินฟราเรดที่รับมา แล้วสั่งทำงานตามแต่ละเงื่อนไข

