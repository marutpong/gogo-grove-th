# 7.8 Using the Remote Control

Making use of the received IR remote commands are done using the Logo commands “newir?” and “ir”. Here is an example:

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

The above program checks if their is a new command from the remote control using the “newir?” in Logo and the “new infrared?” block in Tinker. When true, the infrared code is retrieved using “ir” in Logo and the “get infrared” block in Tinker. This infrared code is stored in the variable “command”. A sequence of “if” statements determine the received code and carries out different actions.

