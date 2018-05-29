# 7.1 มาฝึกเขียนโปรแกรมแรกกัน

โปรแกรมตัวอย่างต่อไปนี้ เป็นคำสั่งให้โกโกบอร์ด ส่งเสียงปิ๊บ 10 ครั้ง ในทุก 1/10 วินาที

```text
to dobeep
    repeat 10 [ beep wait 1] 
end
```

ผู้ใช้สามารถเขียนภาษาโลโก โดยเลือก Tab ที่มีชื่อว่า "Logo" ใน **GoGo Widget** จากนั้นจึงเขียนโค้ดภาษาโลโกลงในพื้นที่ว่างดังรูปประกอบด้านล่าง

![](https://lh6.googleusercontent.com/UEqzAkRPk166KB7GGkmBVv58Zrl8zse01QkX9GZdDacxzmlIHWl3Vsi54iEIZqpf1Ap9NTkvtPuGJFMlAWVoD4DJG8xx6JypWCL7eHC5xtH0Ajcl-lsPRR-D-uu9W7UyBvFSyJgP)

การเขียนโปรแกรมเดียวกัน โดยใช้ Tinker\(เขียนเป็นบล็อกโปรแกรม\):

![](https://lh6.googleusercontent.com/cyfDTmWrIRH_Sd_iB4ONamR53McRD3DA_Y11pbBuhCFtxJYCJwGziTkjMr8op0rxZ2f6AzS0gJGVewzi9bJFJI5DJoc6Qw02oUPZw46fuFO1ykqGg5zJmCfL-2rBf28tEaDZIwbk)

คลิก "**Download**" ใน GoGo Widget หรือ "**Write to GoGo Board**" ใน Tinker เพื่อจะส่งโปรแกรมที่เขียนไปยังโกโกบอร์ด โดยก่อนที่จะส่ง โปรแกรมจะถูกเช็คความถูกต้อง หากพบปัญหาจะมีข้อความแสดงให้แก้ไขให้ถูกต้อง ถ้าโปรแกรมส่งไปยังโกโกบอร์ด เสร็จสมบูรณ์จะมีเสียงปิ๊บหนึ่งครั้ง

{% hint style="info" %}
หากใช้งาน **Tinker** อย่าลืมเปิด **GoGo Widget** ให้ทำงานเบื้องหลังไว้ด้วย เนื่องจาก Tinker มีการใช้งาน **GoGo Widget** ในการสื่อสารกับโกโกบอร์ดที่เชื่อมต่ออยู่
{% endhint %}

ขั้นตอนสุดท้ายคือการรันโปรแกรม ผู้ใช้สามารถรันโปรแกรมได้โดยคลิกปุ่ม "Run/Stop" บน **GoGo Widget** หรือ Tinker นอกจากนั้นยังสามารถกดปุ่ม "Run!" ที่อยู่บนโกโกบอร์ด ได้อีกด้วย ในตัวอย่างนี้เมื่อรันโปรแกรมโกโกบอร์ด จะส่งเสียงปิ๊บ 10 ครั้ง หลอดไฟ "run" LED สีแดงที่อยู่ทางด้านล่างขวาของตัวบอร์ดจะติดขึ้นมาในขณะที่โปรแกรมทำงาน และจะดับลงเมื่อโปรแกรมทำงานเสร็จสิ้น โดยกระบวนการทั้งหมดจะเป็นดังรูปประกอบด้านล่างนี้  


![](https://lh6.googleusercontent.com/q4fQ3aw1q6tOKSh61AeX-r5gI_WmVTXqs4oNkfTB19WJoNNcb3pHJjTRfXb2ajltwEfunIBJc56rxJ96XBANrc9kf1nk46y3cTvYbxXTIPIsS6ekNvcq6Tbt3coAW_oMR1sX0AYt)

{% hint style="info" %}
โปรแกรมที่ Download มายังโกโกบอร์ด จะถูกบันทึกไว้ ถึงแม้ว่าจะไม่ได้เชื่อมต่อกับคอมพิวเตอร์ หรือไม่มีพลังงานเลี้ยงตัวบอร์ด โปรแกรมจะยังคงอยู่และสามารถทำงานได้ โดยจ่ายไฟให้ตัวบอร์ดแล้วกดปุ่ม Run บนตัวบอร์ดได้เลย
{% endhint %}



