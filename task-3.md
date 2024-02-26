By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**
![WhatsApp Image 2024-02-26 at 9 44 10 PM (2)](https://github.com/KMounavi19/KMounavi19/assets/160726381/7a27f79f-772d-4b68-870e-36a245a7143d)
**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&
![WhatsApp Image 2024-02-26 at 9 46 44 PM (1)](https://github.com/KMounavi19/KMounavi19/assets/160726381/cc2f68ff-e2ab-4ece-b2f3-b3baaa8df73b)
Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c
![WhatsApp Image 2024-02-26 at 10 55 36 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/1c55ca37-bd4c-4708-85a8-4e41cff122cd)
Step 5: Check the output by using the command

./a.out
![WhatsApp Image 2024-02-26 at 10 55 36 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/272a7d78-f73c-443a-bd76-2a2d8c2f6099)
The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c
![WhatsApp Image 2024-02-26 at 10 58 17 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/928c3b1e-be1d-49e6-993a-0daf05582d8e)
Step 2: Compile the code in riscv using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c 

![WhatsApp Image 2024-02-26 at 11 07 12 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/f94194c9-7d23-4087-8b91-39ba0e8a6732)

Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command

ls -ltr sum1ton.c

![WhatsApp Image 2024-02-26 at 10 59 50 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/b22debdb-196c-44a8-bc3f-38269e33ebe3)
![WhatsApp Image 2024-02-26 at 11 09 48 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/c261cba1-c86c-4625-a161-1962abc81434)
Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution
![WhatsApp Image 2024-02-26 at 11 11 33 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/888f4b2c-8ad0-4615-88cb-0d1b0979d8cb)
![WhatsApp Image 2024-02-26 at 11 12 19 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/f3a8560a-57cb-4a03-9001-001e22d1670f)
Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![WhatsApp Image 2024-02-26 at 11 14 11 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/a242c490-1dae-477d-954f-1703aba5e232)
![WhatsApp Image 2024-02-26 at 11 14 12 PM](https://github.com/KMounavi19/KMounavi19/assets/160726381/13c5b255-8391-4b90-b0b2-1b220307aa0b)





