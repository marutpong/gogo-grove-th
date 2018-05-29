# 7.6 การเขียนโปรแกรมให้กับหน้าจอแสดงผลบนบอร์ด

ในภาษาโลโก ใช้คำสั่ง "show" ส่วนใน Tinker มีบล็อกแยกต่างหากสำหรับแสดงข้อความหรือตัวเลข ตัวอย่างต่อไปนี้ ต้องการแสดงข้อความ "SS1" บนจอ แล้วรอ 1 วินาที จากนั้นแสดงค่าเซ็นเซอร์ 1 แล้วรออีก 1 วินาที ทำแบบนี้วนไปเรื่อยๆ

{% tabs %}
{% tab title="Logo" %}
```text
to show_sensor
    forever [ 
        show "SS1"
        wait 10 
        show sensor1
        wait 10 
    ]
end
```
{% endtab %}

{% tab title="Tinker" %}
![](https://lh3.googleusercontent.com/9Amo9QLjZEYv0OXgwKuLqudoKyjiTwBqSvfqJdBLFJNHFevZbO1Ef9aQqdnuhZzM-iYuYXb8xcqdRLqTsYbJ3mHUYIoa2H-7vNkYH9lZ3v5DPX_HNS-yWf8I9-q7orZeCoAYw6oS)
{% endtab %}
{% endtabs %}

{% hint style="info" %}
ตรวจสอบให้แน่ใจว่าหน้าจออยู่ในหน้า "User" มิฉะนั้นค่าจากโปรแกรมจะไม่ปรากฏบนจอ[  
](https://docs.gogoboard.cf/th/programming/5_program_control.html)
{% endhint %}

