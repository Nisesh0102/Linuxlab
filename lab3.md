# modifying script

## original script

```
#!/bin/bash        ---shebang
a="Vansh"           ---taking vansh in the variable a
b=40                 ---taking 40 in the variable b

if [ $a="Vansh" ] && [ $b -gt 18 ]; then      ---checking conditions and using an opreator and(&&)
    echo " you are adult "                     ---printing you are adult
fi

if [ $a="Nisesh" ] && [ $b -lt 18 ]; then       ---checking conditions and using an opreator and(&&)
    echo "you are minor"                         --- printing you are minor
fi

```
<img width="572" height="262" alt="Screenshot from 2025-09-08 01-07-53-1" src="https://github.com/user-attachments/assets/d1cedec0-ce33-4a60-8443-f6bf7e4fa9ff" />

<img width="635" height="52" alt="Screenshot from 2025-09-08 01-11-20-1" src="https://github.com/user-attachments/assets/f212ac82-435b-42ee-8736-4b264ebb622a" />


##  modified script

```
#!/bin/bash 
# prompt user for input

read -p "enter your name: " name      --- taking name from the user
read -p "enter your age: " age        --- taking age from the user

if [ $name="Vansh" ] && [ $age -gt 18 ]; then    --- checking conditions with if and opreator and(&&)     
    echo " you are adult "                     --- printing (you are adult)
fi

if [ $name=" Nisesh" ] && [ $age -lt 18 ]; then  ----  checking conditions with if and opreator and(&&)      
    echo "you are minor"                         ---- printing (you are minor)
fi
```
## the difference between the original and modified script is that in the first one we check for fixed value and in the next case we check for all cases .

<img width="611" height="299" alt="Screenshot from 2025-09-08 17-21-03" src="https://github.com/user-attachments/assets/0199893a-7442-40aa-847d-b07c4a1c7896" />


## checking with differnt examples
#### output is :
<img width="554" height="235" alt="Screenshot from 2025-09-08 17-19-45" src="https://github.com/user-attachments/assets/96c69167-3b4e-4ac9-8ba9-cc196bab3074" />


### Q1=differnce between $1,$@ and $# in bash?

Ans-- 0 $1= this refers to positional parameters
         $@= represents all arguments passed to the script
         $#= returns the number of arguments passed

### Q2=what does exit 1 mean in the script
    

Ans-- general error (something went wrong) Or exit with error.
