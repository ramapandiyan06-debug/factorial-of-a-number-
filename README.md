# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```asm
ORG 0000H
MOV DPTR,#4500H
MOVX A,@DPTR
MOV R0,A
INC DPTR
ACALL FACTORIAL
MOVX @DPTR,A
SJMP THIN
FACTORIAL:DEC R0
CJNE R0,#01H,PRODUCT
SJMP THICK
PRODUCT:MOV B,R0
MUL AB
ACALL FACTORIAL
THICK: RET
THIN:RET
END

```
OUTPUT

<img width="957" height="190" alt="553299198-28b10bcb-eaf3-4ad4-a951-c374f684d200" src="https://github.com/user-attachments/assets/7d683fe3-c592-4aa8-9a98-a3abe0774e22" />


---
MANUAL CALCULATIONS

![WhatsApp Image 2026-02-26 at 4 11 04 PM](https://github.com/user-attachments/assets/c722265d-7245-47d0-ab4e-0be09806e53b)


RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---


