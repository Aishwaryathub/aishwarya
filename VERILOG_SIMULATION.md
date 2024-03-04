# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I

![b2](https://github.com/Aishwaryathub/aishwarya/assets/160737960/f0edbf3c-84e1-4620-a4e8-8351c8e61c76)

## 3. INSTRUCTION SET OF RISC-V RV32I
![b3](https://github.com/Aishwaryathub/aishwarya/assets/160737960/28e744ea-c286-45e7-81fc-a8f6b9d80ffd)
![b3 1](https://github.com/Aishwaryathub/aishwarya/assets/160737960/05fbb270-9fb2-4cda-a467-0215c0bf981b)

## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**
 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```
![WhatsApp Image 2024-03-02 at 6 18 33 PM](https://github.com/Aishwaryathub/aishwarya/assets/160737960/0af13343-d870-40f4-887c-aac6358937ef)

- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**
$ git clone https://github.com/aishwaryathub/aishwaryathub.git
$ cd aishwarya
![b4](https://github.com/Aishwaryathub/aishwarya/assets/160737960/7c65e3c6-1d1d-4e72-8b96-fe90104882ef)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![WhatsApp Image 2024-03-02 at 6 18 33 PM](https://github.com/Aishwaryathub/aishwarya/assets/160737960/70ec08e0-4d23-4dd5-8e5b-8e646fc85b02)

- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`
![WhatsApp Image 2024-03-02 at 6 18 33 PM](https://github.com/Aishwaryathub/aishwarya/assets/160737960/33b86523-2a46-493f-8947-da02504372e1)

### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 ![o1](https://github.com/Aishwaryathub/aishwarya/assets/160737960/8ceff2a2-8966-4058-807e-f184f3f6913f)

Instruction 2:sub r7,r1,r2
![o2](https://github.com/Aishwaryathub/aishwarya/assets/160737960/ddc30eb3-1bcf-4589-afc7-246b4b0c4bbb)

Instruction 3:and r8,r1,r3
![o3](https://github.com/Aishwaryathub/aishwarya/assets/160737960/07cdd08b-af66-4ce0-b63c-65db1478ee5b)

Instruction 4:or r9,r2,r5
![o4](https://github.com/Aishwaryathub/aishwarya/assets/160737960/43f2ad5c-1987-472e-a56e-00e07f7ee49e)

Instruction 5:xor r10,r1,r4
![5](https://github.com/Aishwaryathub/aishwarya/assets/160737960/dbc44ab1-99b3-4a15-aa28-3b42db74014c)

Instruction 6:slt r11,r2,r4
![o6](https://github.com/Aishwaryathub/aishwarya/assets/160737960/4fd965e3-1106-488c-9ac5-947d19fcdfee)

Instruction 7:addi r12,r4,5
![o7](https://github.com/Aishwaryathub/aishwarya/assets/160737960/849746de-63c5-4fb7-a2e8-6f4914bd8c50)

Instruction 8:sw r3,r1,2
![o8](https://github.com/Aishwaryathub/aishwarya/assets/160737960/e628f31d-1672-4a60-ba0a-63b581db723c)

Instruction 9:lw r13,r1,2
![o9](https://github.com/Aishwaryathub/aishwarya/assets/160737960/e330c7fa-0f96-4f5a-a06b-805367436adf)

Instruction 10:beq r0,r0,15
![o10](https://github.com/Aishwaryathub/aishwarya/assets/160737960/c0cfb9a3-0427-4168-946c-755b3c3b8da5)

 After branching, performing
 Instruction 11:add r14,r2,r2
 ![o11](https://github.com/Aishwaryathub/aishwarya/assets/160737960/10dc6aa7-7f5b-4e68-961e-42c158c2bf5e)

Full 5-stage instruction pipeline and pc-increment description Waveform
![o12](https://github.com/Aishwaryathub/aishwarya/assets/160737960/7b9f99e5-beac-4451-9662-a2a253fcf695)
![WhatsApp Image 2024-03-02 at 6 18 33 PM (3)](https://github.com/Aishwaryathub/aishwarya/assets/160737960/77a14377-59e7-443d-b68e-8c77445b09ab)
![WhatsApp Image 2024-03-02 at 6 18 33 PM (6)](https://github.com/Aishwaryathub/aishwarya/assets/160737960/793d94d7-0b34-4dc3-9196-b14c969414b8)


 
