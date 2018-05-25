# 7.7 Using Variables

A variable is a powerful tool that allows a program to count, store data, define values and much more. The following example shows how a variable can be used to count the number of times a switch is pressed and shows the number on the GoGo Board’s screen. Connect a switch to sensor port 1 and run the following program.

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

![](https://lh6.googleusercontent.com/YIcKKPd6BdOsRpyhiBmMULTE1wGTkAPrzFzVu0PwLzO2FmxM390GV1zfk6d9Y0WIgp1UI10WL6AZ0KgDUuwC-yiu1cZ6YIk-h0Z2yUOYrWWILc1sBrV_z8AejLNQ2iYshJgdFvjy)

The set command is used to assign a value to a variable. In the above example, the program starts by setting a variable named “counter” to 0. Note that this initial setting also makes the variable name valid and available for use in the rest of the program. In Logo the variable name “counter” can be used as an argument for any command that takes an expression as an input.

In Tinker, variables are listed in the section “Variables” and can be managed from there. To create a new variable, drag a “set” block onto the programing area. Then, click the drop-down button and there will be menus to either rename that variable or create a new one.

![](https://lh3.googleusercontent.com/5at4y_DcVZyn-h1WJaH5GqmF5772E-W9qP6dY01BqZDlH7DH6GXHfvr8qRZ0Xc8t75S6OckO79i0BGjO-qSpvwxujLyUm1KEMc-8bQvx7G45NJlBWzfy01dne1PgFViZoUmuWVk7)

