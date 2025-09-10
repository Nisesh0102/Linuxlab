# 🔧understanding how existing scripts in repo work

# 🔧script 1

  ```
 #!/bin/bash      - shebang
 echo "hello world!"     - printing hello world
 name="Nisesh Singh"   - taking Nisesh Singhvin variable name
 age=18    -  taking 18 in variable age 

 echo "My name is $name ansd I am $age year old."  - printing name and age
```
#### OUTPUT :
<img width="778" height="173" alt="Screenshot from 2025-09-08 00-43-35" src="https://github.com/user-attachments/assets/a4703c21-cf08-4f84-9d56-f88bb486cf3b" />

<img width="622" height="73" alt="Screenshot from 2025-09-08 00-44-11" src="https://github.com/user-attachments/assets/597ec280-7558-41f7-aa03-22582656034b" />



# 🔧 script 2

```
#!/bin/bash        -shebang
a="Nisesh Singh"           -taking Nisesh Singh in the variable a
b=40                 -taking 40 in the variable b

if [ $a="Nisesh Singh" ] && [ $b -gt 18 ]; then      -checking conditions and using an opreator and(&&)
    echo " you are adult "                     - printing you are adult
fi

if [ $a="Vansh" ] && [ $b -lt 18 ]; then       -checking conditions and using an opreator and(&&)
    echo "you are minor"                         - printing you are minor
fi

```
<img width="572" height="262" alt="Screenshot from 2025-09-08 01-07-53" src="https://github.com/user-attachments/assets/e26d5619-5d46-4f8f-9e55-bf8ff0aed544" />

<img width="635" height="52" alt="Screenshot from 2025-09-08 01-11-20" src="https://github.com/user-attachments/assets/d5cfc882-2d7c-4148-b7f7-3bce324c5901" />



### 🔧 Q1 what is the purpose of #!/bin/bash at the top of the script

ANS-- the shebang line at the top of a script specifies the interpreter that should be used to the run the script.

### 🔧 Q2 how do you make a script executable?
ANS-- 1. add the shebang at the top
          2. give permission using the chmod command

          3. run the code.

