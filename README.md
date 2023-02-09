# BASH
**BASH Scripting For Beginners**

![BASH](https://opensource.com/sites/default/files/lead-images/bash_command_line.png)

**What is BASH ?**
> Bash is a Unix shell and command language written by Brian Fox for the GNU Project as a free software replacement for the Bourne shell.

**Types Of Shells**

```
1. BASH
2. ZSH
3. TSH
4. CSH
5. KSH
6. Fish
```

**1. Text Formatting**

```
#!/usr/bin/bash
#Use echo to print texts
echo "Hello World"
```

**2. Color Patterns**

```
#!/usr/bin/bash
#Use -e option to add colours to text
echo -e "\e[1;31mHello World\e[0m"
```
>Colour Codes

| Color | Text Color | Background Color |
|--|--|--|
| Red | 31m | 41m |
| Green | 32m | 42m |
| Yellow | 33m | 43m |
| Blue | 34m | 44m |
| Magenta | 35m | 45m |
| Cyan | 36m | 46m |
| Light Gray | 37m | 47m |
| Gray | 90m | 100m |
| Light Red | 91m | 101m |
| Light Green | 92m | 102m |
| Light Yellow | 93m | 103m |
| Light Blue | 94m | 104m |
| Light Magenta | 95m | 105m |
| Light Cyan | 96m | 106m |
| White | 97m | 107m |

**3. Variables **
>Three Types Of Variables in **BASH**
```
1. System  Declared Variables
2. Programmer Declared Variables
3. Command Line Argument
```

**Programmer Declared Variable**

>We can use $ to declare a variable

```
#!/usr/bin/bash
#Declare name as Yell Phone Naing
name="Yell Phone Naing"
echo "My name is $name"
```
