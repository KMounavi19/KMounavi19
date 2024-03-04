As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
Veriog code is being executed and the waveforms are generated using the gtkwave
Aim: To verify the Functional Simulation:-
Table of contents
1.RISC-V RV32I

2.BLOCK DIAGRAM OF RISC-V RV32I

3.INSTRUCTION SET OF RISC-V RV32I

4.FUNCTIONAL SIMULATION

4.1 About iverilog and gtkwave
4.2 Installing iverilog and gtkwave
4.3 The output waveform
1. RISC-V RV32I
This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

2. BLOCK DIAGRAM OF RISC-V RV32I
   ![WhatsApp Image 2024-03-04 at 10 02 06 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/3fc4ae9f-5f39-4383-8169-cb97c1fd94d9)
3. INSTRUCTION SET OF RISC-V RV32I
![WhatsApp Image 2024-03-04 at 10 03 55 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/75f9bb5d-e927-4da9-9d32-505f51996a9f)
![WhatsApp Image 2024-03-04 at 10 06 16 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/58e89cee-b051-4444-b959-750af91bff6f)

4. FUNCTIONAL SIMULATION
4.1 About iverilog and gtkwave
Icarus Verilog is an implementation of the Verilog hardware description language.
GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing

4.2 Installing iverilog and gtkwave
For Ubuntu
Open your terminal and type the following to install iverilog and GTKWave

$   sudo apt get update
$   sudo apt get install iverilog gtkwave
![WhatsApp Image 2024-03-04 at 10 10 57 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/1280e518-1772-462a-a692-11612e180460)
To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.
$ git clone https://github.com/KMounavi19/KMounavi19
$ cd KMounavi19
![WhatsApp Image 2024-03-04 at 10 15 41 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/f93104bf-6353-433d-a4a7-c57739fd5b55)
To simulate and run the Verilog code, enter the following commands in your terminal.
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
![WhatsApp Image 2024-03-04 at 10 23 05 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/32cfed85-9ee6-4a90-8cca-626cb04ac0f4)
To see the output waveform in gtkwave, enter the following commands in your terminal.
$ gtkwave hello.vcd
![WhatsApp Image 2024-03-04 at 10 30 53 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/52acea0a-5ae9-4b90-a683-fb48c87ba0ff)
4.3 The output waveform
The output waveform showing the instructions performed in a 5-stage pipelined architecture.

Instruction 1:add r6,r2,r1
![WhatsApp Image 2024-03-04 at 10 43 56 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/4329f40a-466a-4b28-9387-895e081c4063)
Instruction 2:sub r7,r1,r2
![WhatsApp Image 2024-03-04 at 10 45 36 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/f1eaa003-14cd-461e-9eff-079ff95a27ce)
Instruction 3:and r8,r1,r3
![WhatsApp Image 2024-03-04 at 10 48 08 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/b61fb8f7-7cea-4623-9236-59661b460bc2)
Instruction 4:or r9,r2,r5
![WhatsApp Image 2024-03-04 at 10 50 34 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/7701a35c-b71e-4ccb-b7c6-0fc94be536f5)
Instruction 5:xor r10,r1,r4 
![WhatsApp Image 2024-03-04 at 10 52 25 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/80d9822e-814d-4a8e-9b61-836877443861)
Instruction 6:slt r11,r2,r4
![WhatsApp Image 2024-03-04 at 10 54 06 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/48b6acc8-99d2-4765-b234-837f8eafebce)
Instruction 7:addi r12,r4,5
![WhatsApp Image 2024-03-04 at 10 55 43 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/4b4901bd-eb49-4b61-878a-99280852e869)
Instruction 8:sw r3,r1,2
![WhatsApp Image 2024-03-04 at 10 57 15 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/3aa9f8e5-6501-497e-ad7f-03dd739da744)
Instruction 9:lw r13,r1,2
![WhatsApp Image 2024-03-04 at 10 57 15 PM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/0ca322e2-926e-457c-9ab8-74c58f76b455)
Instruction 10:beq r0,r0,15 
![WhatsApp Image 2024-03-04 at 11 00 00 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/300ccc44-76c8-427e-8a19-5083a6298df3)
After branching, performing Instruction 11:add r14,r2,r2
![WhatsApp Image 2024-03-04 at 11 00 00 PM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/5b06566f-7baf-4c09-b272-a9f0497a13c8)
Full 5-stage instruction pipeline and pc-increment description Waveform
![WhatsApp Image 2024-03-04 at 11 03 38 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/4105811b-26f2-4022-9313-17037da86c3a)
![WhatsApp Image 2024-03-04 at 11 05 26 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/857bb649-c9ca-483c-bda8-2ce76424858c)
![Screenshot from 2024-03-04 23-10-32](https://github.com/KMounavi19/KMounavi19/assets/160726381/f3f94246-16ba-40b5-a573-56a083fc6109)


