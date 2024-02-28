Meeting Held on: 27/02/2024

The C code should undergo the simulation of normal GCC X86 Compiler and riscv compiler (SPIKE Simulation)

AS PER THE REQUIREMENT OUTPUT OF GCC (F1) SHOULD BE EQUAL = TO OUTPUT OF RISCV GCC (F2)
![WhatsApp Image 2024-02-28 at 10 45 01 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/ff5d441b-823d-488d-b724-ebbb1003156c)

Step - 1:Run the code in the normal GCC Compiler To compile the code: gcc sum1ton.c -o sum1ton To Get the output use "./a.out" : Here the output finds to be -Sum of numbers from 1 to 50 is 125250

Step - 2: To Run the code in the RISC-V GCC Compiler

To compile the code: riscv64-unknown-elf-gcc -o sum1ton sum1ton.c To Get the output use "./a.out" : Here the output finds to be -Sum of numbers from 1 to 50 is 125250
![Screenshot from 2024-02-28 22-26-26](https://github.com/KMounavi19/KMounavi19/assets/160726381/01ec65cc-041d-46eb-8406-da10228b37ba)
![Screenshot from 2024-02-28 22-29-49](https://github.com/KMounavi19/KMounavi19/assets/160726381/5ba7f502-c352-4c30-9f1e-d829bea3de0d)
![Screenshot from 2024-02-28 22-29-49](https://github.com/KMounavi19/KMounavi19/assets/160726381/d7c9eda4-e611-4a55-a12a-e248d247d3ab)
