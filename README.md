# ASSIGNMENT
## AIM

Write a 8051 c program to generate a square wave with frequency of 50khz
---

## APPARATUS REQUIRED

* Personal Computer with KEIL Software

---
#### Program

```
#include <reg51.h>   
void delay(unsigned int);  
void main() {
    while(1) {
        P0 = 0x00;      
        delay(6);       
        P0 = 0xFF;      
        delay(6);       
    }
}
void delay(unsigned int count) {
    unsigned int i, j;
    for(i = 0; i < count; i++)
        for(j = 0; j < 1000; j++); 
}

```


---

## OUTPUT IMAGE FROM KEIL SOFTWARE
<img width="1919" height="927" alt="image" src="https://github.com/user-attachments/assets/dac4b464-6569-4dbd-ac2d-c3e31fab5487" />







------------------------------------------------
### IN ASSEMBLY LANGUAGE
## AIM

Write a 8051 program to generate a square wave with frequency of 50khz
---

## APPARATUS REQUIRED

* Personal Computer with KEIL Software

---
#### Program

```
ORG 0000H
L1:MOV A, #00H      
MOV P0, A
MOV R0, #6   
L2: DJNZ R0,L2
MOV A, #0FFH      
MOV P0, A
MOV R0, #6        
L3: DJNZ R0,L3
SJMP L1      
END
```


---

## OUTPUT IMAGE FROM KEIL SOFTWARE
<img width="1919" height="865" alt="image" src="https://github.com/user-attachments/assets/d9f3464f-4a9e-4ec8-80e6-0f24417f0d22" />
