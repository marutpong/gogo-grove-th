# 7.6 Programming the Built-in Screen

In Logo, use the show command. In Tinker, there are separate blocks for showing text and numbers. The following example repeatedly displays the text “SS1” and then followed by sensor 1’s value.

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
Make sure the screen is in the “User” page. If not, the values from the program will not be seen.
{% endhint %}



