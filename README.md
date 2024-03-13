# OpenRISC
## VSDsquadron Internship

This repository is intended to document the learning outcomes and experience of a 4-week workshop on RISC-V.

#### TASK 1: 

1. Create GitHub repo. 
2. Need to have Windows OS, 1TB HDD, 16GB RAM.
3. Allocate 8GB RAM, 100GB HDD for Oracle Virtual Machine 
4. install RISC-V GNU Toolchain first, then install Yosys, iverilog, gtkwave. 
5. Refer to this course :VSD - A complete guide to install open-source EDA tools to install Ubuntu 20.04 using Virtual Box




#### installation of IVERILOG

```
sudo apt update
sudo apt install iverilog

```
![image](https://github.com/ajishza/openrisc/assets/73847946/445d0812-2878-4d35-9c5c-2db3486c259a)
---
#### installation of  gcc compiler
```
sudo apt install git-all 
sudo apt-get install autoconf automake autotools-dev curl python3 python3-pip libmpc-dev libmpfr-dev libgmp-dev gawk build-essential bison flex texinfo gperf libtool patchutils bc zlib1g-dev libexpat-dev ninja-build git cmake libglib2.0-dev
git clone https://github.com/riscv/riscv-gnu-toolchain --recursive
mkdir riscv 
chmod -R 777 /home/work/riscv
./configure --prefix=/home/work/riscv

```



#### task 2

There are 6 instruction formats 
1. Register type formats : This uses 3 register inputs Eg : add, mul, AND - All are basically arithmetic and logical operations
 Eg: add r6,r2,r1   r1 and r2 are source registers and r6 is destination register
2: I-type: immediate and load operations 
Eg: addi r12,r4,5
    lw x14,x2,8
3. S-type: store operations 
Eg: sw x12, x2,8
4. B-type: conditional branch operations 
Eg: beq r0, r0 ,15
    bne r0, r1,20
5. U-type: long immediate operation

   INSTRUCTION	INSTRUCTION TYPE	32 BIT CODE
add r6, r2, r1	R	0000000	00001	00010	000	00110	0110011

sub r7, r1, r2	R	0100000	00010	00001	000	00111	0110011


and r8, r1, r3	R	0000000	00011	00001	111	01000	0110011


or r9, r2, r5
	R	0000000	00101	00010	110	01001	0110011

xor r10, r1, r4
	R	0000000	00100	00001	100	01010	0110011

slt r11, r2, r4
	R	0000000	00100	00010	010	01011	0110011

addi r12, r4, 5	I	0000000	00100	01100	0000000000000101	0010011


sw r3, r1, 2
	S	0000000	00001	00011	010	00010	0100011

lw r13, r1, 2
	I	0000000	00001	01101	010	00010	0000011

beq r0, r0, 15
	B	0001000	00000	00000	0000000000001111	1100011

bne r0, r1, 20
	B	0001011	00000	00001	0000000000010101	1100011

sll r15, r1, r2(2)
		0000000	00010	00010	001	00010	0010011


0000000	00010	01111	001	00010	0110011


srl r16, r14, r2(2)
		0000000	00010	00010	001	00010	0010011


0000000	01110	10000	101	00010	0110011


                                         


 - 
#### task 3
 - C Lab  & OPENRISC assigmnment
 - Refer Iverilog.doc
#### task 4
-  Spike simulataion
-  Refer the document spike_simulation.docx
   

