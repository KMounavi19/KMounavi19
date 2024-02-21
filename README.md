A 4-week Research Internship on RISC-V using VSDSquadron Mini RISC-V Dev Board BOARD SPECS:

CH32V003F4U6 chip with 32-bit RISC-V core based on RV32EC instruction set

SRAM 2kb onchip volatile sram 16kb external program memory
Processor 24 MHz
Sink Current per I/O Pin 8 mA
Source Current per I/O Pin 8 mA
Input voltage (nominal) 5 V
I/O voltage 3.3 V
Programmer/debugger Onboard RISC-V programmer/debugger, USB to TTL serial port support
SPI 1x, PC5(SCK), PC1(NSS), PC6(MOSI), PC7(MISO)
I2C 1x, PC1(SDA), PC2(SCL)
USART 1x, PD6(RX), PD5(TX)
External interrupts 8 external interrupt edge detectors, but it only maps one external interrupt to 18 I/O ports
PWM pins 14X
Analog I/O pins 10-bit ADC, PD0-PD7, PA1, PA2, PC4
Digital I/O pins 15
Built-in LED Pin 1X onboard user led (PD6)
USB 2.0 Type-C
TASK 1:

1.To install RISC-V GNU Tool chain


sudo apt install git-all # To install git
sudo apt-get install autoconf automake autotools-dev curl python3 libmpc-dev libmpfr-dev libgmp-dev gawk build-essential bison flex texinfo gperf libtool patchutils bc zlib1g-dev libexpat-dev
git clone https://github.com/riscv/riscv-gnu-toolchain

![WhatsApp Image 2024-02-21 at 10 43 25 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/f99c60fe-ea48-44ae-8d69-6cff50d8d494)
![WhatsApp Image 2024-02-21 at 10 47 22 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/6539f542-f1a6-4d0f-ad95-6f6b5b46208a)
![WhatsApp Image 2024-02-21 at 10 48 54 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/2374c1a7-bb02-427f-afa0-6d05058868e4)


2.To install Yosys

git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt-get install build-essential clang bison flex \libreadline-dev gawk tcl-dev libffi-dev git \ graphviz xdot pkg-config python3 libboost-system-dev\libboost-python-dev libboost-filesystem-dev zlib1g-dev
sudo apt-get install tcl-dev
sudo apt-get install libreadline-dev!
make config-gcc!
make
sudo make install
![WhatsApp Image 2024-02-21 at 10 55 39 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/0a2377fe-a3d8-4607-af11-e0b0a4ce30a4)
![WhatsApp Image 2024-02-21 at 10 57 27 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/01f80a53-3865-4543-9daa-16ac394ff800)
![WhatsApp Image 2024-02-21 at 10 57 28 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/46324e08-ae17-4f22-b10b-60f152e271a8)

3.To install iverilog and gtkwave

sudo apt-get install iverilog
sudo apt update
sudo apt-get install gtkwave
![WhatsApp Image 2024-02-21 at 11 07 06 PM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/37429fbc-9e03-4df8-aef9-3c25418a1a94)
![WhatsApp Image 2024-02-21 at 11 09 00 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/c15ef9c5-fd4f-4607-870e-681a53d0a5c6)











