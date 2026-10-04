## sub1.asm

eax shows **226 (unsigned value)**, signed value would be **-30**

**flags [CF PF SF IF]**

* **IF** allows for maskable interrupts to be serviced
* **CF** - there was need for unsigned borrowing
* **SF** - the msb was 1 (which shows that the result was negative for signed operations)
* **OF** was not set because the signed result fit in the 8bits


## sub2.asm

eax shows **64536 (unsigned value)**, signed value would be **-1000**

**[CF PF SF IF]**

* **CF** - there was need for unsigned borrowing
* **SF** - negative number (if signed) because the msb was 1
* **PF** - even number of 1's in the lower 8 bits
* **OF** was not set because the result fit in the given 16 bits
