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
 - 
#### task 3
 - C Lab  & OPENRISC assigmnment
 - Refer Iverilog.doc
#### task 3
-  Spike simulataion
-  Refer the document spike_simulation.docx
   

