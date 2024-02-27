# task 0
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
