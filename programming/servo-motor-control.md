# 7.4 Servo Motor Control

Controlling a servo motor usually means setting the desired motor position. The command to perform this action in Logo is “seth” which stands for “set heading”. In Tinker, use the block “Set servo heading”. Consider the following example:

{% tabs %}
{% tab title="Logo" %}
```text
to servo_control
    a, seth 10
    wait 10
    seth 40
end
```
{% endtab %}

{% tab title="Tinker" %}
![](https://lh4.googleusercontent.com/PkmsY5-cdQdVwbAopSlrqHpR7Jv5qdOaXAQBVsUFYRu2SJNSxbpRt7mhYs3Hy20a6yt_RV5rIIBncz3jdMnbty0fHZ75TYTb4vwGAmCdNQRIMrX3-MDVclbIgTv-_xJMFzDH39Qe)
{% endtab %}
{% endtabs %}

The above example will turn a servo motor connected to servo port A to the heading position “10”, wait for 1 second and then turn the servo to the heading position “40”.

Position 10 Position 40

![](https://lh5.googleusercontent.com/xtZp4ZZl4JNFAgu8kyWSmIFpz0SxSFi2ntoOE3QUd8pL_MhZELgxHFgT0YgFS0w38-FUdsYMNWRx0kAqkeN9XruZ7gXuftvatO05IDgA-FmVsGJd-sIU-IKQD3q_PyMbPxiQhq9k)

## Servo Motor Heading Position {#servo-motor-heading-position}

The heading positions “10” or “40” in the example does not correspond to a standard angle or unit. It is a GoGo Board internal position number. Therefore, you need to determine what number to use so that the motor points to the desired direction. This is easily done using the GoGo Widget’s manual servo controls as described earlier.

{% hint style="warning" %}
Do not use a heading position that exceeds the bounds of the servo. Since servos do not rotate a full circle, exceeding the heading bounds could break the internal gearings of the servo. Although different servo models and brands have slight variations but, typically, the heading value should stay between 10 - 40.
{% endhint %}

