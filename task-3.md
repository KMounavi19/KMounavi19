By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**
![WhatsApp Image 2024-02-27 at 11 31 19 AM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/9d8e6c42-cdb4-43ec-8603-e4a1dc9545b1)
**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&
![WhatsApp Image 2024-02-27 at 11 31 58 AM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/3f4bf63c-f707-4383-8108-37566409bdd1)
Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c
![WhatsApp Image 2024-02-27 at 11 34 21 AM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/abefa05a-21e7-43f0-90f6-25294273c9a6)
Step 5: Check the output by using the command

./a.out
![WhatsApp Image 2024-02-27 at 11 36 35 AM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/c1d969c1-6697-4984-b566-c963c4570a1a)
The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c
![WhatsApp Image 2024-02-27 at 11 37 42 AM (2)](https://github.com/KMounavi19/KMounavi19/assets/160726381/e9fd5a12-d231-4b8c-84ac-106dafd68b31)
Step 2: Compile the code in riscv using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![WhatsApp Image 2024-02-27 at 11 38 21 AM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/27c5bf83-bd3a-4018-8062-623cc1238bda)
Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command
ls -ltr sum1ton.c
![WhatsApp Image 2024-02-27 at 11 39 32 AM](https://github.com/KMounavi19/KMounavi19/assets/160726381/4fc1d790-a2b9-4347-878e-21766fa5972f)
![WhatsApp Image 2024-02-27 at 11 40 25 AM](https://github.com/KMounavi19/KMounavi19/assets/160726381/3caa7014-ee73-41f3-bbb1-1bf7b6b2dff1)
Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution
![WhatsApp Image 2024-02-27 at 11 43 02 AM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/ad24c62e-96c9-4c63-a7ec-28e14b875606)
![WhatsApp Image 2024-02-27 at 11 43 02 AM (2)](https://github.com/KMounavi19/KMounavi19/assets/160726381/efcfbb2b-dec0-469f-bc7d-1feaa217cd9f)
Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![WhatsApp Image 2024-02-27 at 11 43 02 AM (3)](https://github.com/KMounavi19/KMounavi19/assets/160726381/b54d4579-72b0-4be2-9903-a745ad3f6d5c)
![WhatsApp Image 2024-02-27 at 11 43 02 AM (4)](https://github.com/KMounavi19/KMounavi19/assets/160726381/97534c6c-d048-4d18-8932-ea2c494f22d1)








