# OpenRISC
## VSDsquadron Internship

This repository is intended to document the learning outcomes and experience of a 4-week workshop on RISC-V.

#### TASK 1: 

1. Create GitHub repo. 
2. Need to have Windows OS, 1TB HDD, 16GB RAM.
3. Allocate 8GB RAM, 100GB HDD for Oracle Virtual Machine 
4. install RISC-V GNU Toolchain first, then install Yosys, iverilog, gtkwave. 
5. Refer to this course :VSD - A complete guide to install open-source EDA tools to install Ubuntu 20.04 using Virtual Box




# installation of tools

```
sudo apt update
sudo apt install iverilog

```
![image](https://github.com/ajishza/openrisc/assets/73847946/445d0812-2878-4d35-9c5c-2db3486c259a)
---
## installation of  gcc compiler
```
sudo apt install git-all 
sudo apt-get install autoconf automake autotools-dev curl python3 python3-pip libmpc-dev libmpfr-dev libgmp-dev gawk build-essential bison flex texinfo gperf libtool patchutils bc zlib1g-dev libexpat-dev ninja-build git cmake libglib2.0-dev
git clone https://github.com/riscv/riscv-gnu-toolchain --recursive
mkdir riscv 
chmod -R 777 /home/work/riscv
./configure --prefix=/home/work/riscv

```
### OpenSTA


#### task 1
 - Instruction Type 
 - instuction byte
 - Refer Instructioncode_updated.docx
#### task 2
 - C Lab  & OPENRISC assigmnment
 - Refer Iverilog.doc
#### task 3
-  Spike simulataion
-  Refer the document spike_simulation.docx
   

