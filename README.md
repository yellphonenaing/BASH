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

# Linux Command syntax
| Character | Action |
|--|--|
| && | And |
| \|\| | Or |
| \| | Give Output To Second Command |

```
ls -lah /tmp
```
>ls = command to be executed, -lah = Options, /tmp = ARgument


# 1. Text Formatting

```
#!/usr/bin/bash
#Use echo to print texts
echo "Hello World"
```

# 2. Color Patterns

```
#!/usr/bin/bash
#Use -e option to add colours to text
echo -e "\e[1;31mHello World\e[0m"
```

>Style Codes

|Code | Style |
|--|--|
| 0 | Normal |
| 1 | Bold |
| 2 | Faint |
| 3 | Italics |
| 4 | Underlined |
| 4 | Blink |

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

# 3. Variables

>Three Types Of Variables in **BASH**
```
1. System  Declared Variables
2. Programmer Declared Variables
3. Command Line Argument
```

**3.1 System Declared Variables**

| Variable | Value |
|--|--|
| $0 | Script File Name (or) Shell Name |
| $$ | Process ID Of Running BASH Script|
| $PWD | Current Directory |
| $OLDPWD | Old Directory |
| $FUNCNAME | Funcation Name |
| $BASH_VERSION | Version Of BASH |
| $HOSTNAME | Host Name |
| $OSTYPE | Type Of OS |
| $RANDOM | Random Number Between 0 and 32767 |


**3.2 Programmer Declared Variable**

```
#!/usr/bin/bash
#Declare name as Yell Phone Naing
name="Yell Phone Naing"
echo "My name is $name"
```

**3.3 Command Line Argument**

```
#!/usr/bin/bash

echo "My name is $1.I am $2 years old.I live in $3."
```

>Run script as bash script.sh YPN 20 Malun


>**Output :** My name is YPN.I am 20 years old.I live in Malun.

# 4. Redirections

>Two Types Of Redirections
```
1. Truncate Redirection
2. Append Redirection
```

**4.1 Truncate Redirection**
>We can use > to perform Truncate Redireection

```
ls > fileslist.txt
```

**4.2 Append Redirection**
>We can use >> to perform Append Redireection

```
echo "Python" >>languages.txt
echo "PHP" >>languages.txt
echo "BASH" >>languages.txt
echo "Ruby" >>languages.txt
```

# 5. User Prompts
>User prompt is an input used to get data from user.

>Normal Prompt
```
#!/usr/bin/bash
echo "Enter your name :: " name
read name
echo "Your name is $name"
```

>Prompt with paragraph
```
#!/usr/bin/bash
read -p "Enter your name : " name
echo "Your name is $name"
```


>Password Input
```
#!/usr/bin/bash
read -s -p "Enter your password : " password
echo -e "\nYour password is $password"
```

>Prompt with color
```
#!/usr/bin/bash
read -p $'\e[1;32mEnter your name : \e[0m' name
echo "Your name is $name"
```

# 6. Conditional Statements
>The conditional statement is used in any programming language to do any decision-making tasks.

>if else statement
```
#!/usr/bin/bash
if [ 1 == 1 ];then
echo "Equal"
else
echo "Not Equal"
fi
```

>if elif else statement
```
#!/usr/bin/bash
if [ 20 == 1 ];then
echo "Equal"
elif [ 20 = 20 ];then
echo "20 = 20 is true"
else
echo "Not Equal"
fi
```

>if else shortcut
```
#!/usr/bin/bash
[[ "Yell Phone Naing" == "Yell Phone Naing" ]] && echo "True"
[[ "Yell Phone Naing" == "CyberBullet" ]] || echo "False"
```
