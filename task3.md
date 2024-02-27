By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**

![Screenshot from 2024-02-27 10-24-22](https://github.com/Aishwaryathub/aishwarya/assets/160737960/72f52b77-decc-4183-b420-a9f4e1f955ba)
**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&
![Screenshot from 2024-02-27 10-24-07](https://github.com/Aishwaryathub/aishwarya/assets/160737960/ef96d2bf-c012-435f-a542-f1da9a84af7d)

Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c

Step 5: Check the output by using the command

./a.out

The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c

**Step 2: Writing the C code in the leafpad editor using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c


Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command
ls -ltr sum1ton.c


![step4](https://github.com/Aishwaryathub/aishwarya/assets/160737960/decc55ed-40de-4d8e-93c1-fe3f09a5f0b3)

Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution

![1](https://github.com/Aishwaryathub/aishwarya/assets/160737960/211048b2-ccb9-48f0-a151-aa13afd3e21e)

![2](https://github.com/Aishwaryathub/aishwarya/assets/160737960/ebb83580-97ae-46a9-96a4-a0d7d7da3b2e)

Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![3](https://github.com/Aishwaryathub/aishwarya/assets/160737960/4bea9029-2bb2-4f0d-a580-975be659078f)

![4](https://github.com/Aishwaryathub/aishwarya/assets/160737960/91a51236-0792-4ee2-b7c7-31c32859d05d)
