# ASSIGNMENT
## AIM

Write a 8051 c program to generate a square wave with frequency of 50khz
---

## APPARATUS REQUIRED

* Personal Computer with KEIL Software

---
#### Program

```
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,1200H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
JNC L1
INC CL
L1:MOV [SI+04H],AX
MOV [SI+06H],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```


---

## OUTPUT IMAGE FROM KEIL SOFTWARE







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
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,1200H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
JNC L1
INC CL
L1:MOV [SI+04H],AX
MOV [SI+06H],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```


---

## OUTPUT IMAGE FROM KEIL SOFTWARE
