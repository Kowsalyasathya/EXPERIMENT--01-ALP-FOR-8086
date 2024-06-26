### Name : Kowsalya M
### Roll no : 212222230069

# EXPERIMENT 01 ALP FOR 8086
## Aim: 
To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 
8086  emulator 
## Theory 

Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.

## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color
  
3.	write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 
6.	Click OK to see/view the output of your program on the Emulator screen. 
7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 

![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)

9.	Click on emulate to start emulation 

![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)


10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 

![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)

## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
org 100h

mov ax,8h;
mov bx,7h;
add ax,bx;
mov [2345h],ax;

ret
```
## Output  
![Screenshot 2024-02-20 154400](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/0daa8dbb-0134-489f-9531-d44d3822354c)

## Subtraction   of 8 bit numbers  ALP 
 ```
org 100h

mov al,9h;
mov bl,6h;
sub al,bl;
mov [7895h],al;

ret
```
## Output :
![Screenshot 2024-02-20 155431](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/f8289504-d887-40f0-a211-eff9e268fcd8)

## Multiplication alp :
```
org 100h

mov ax,0b548h;
mov bx,0a178h;
mul bx;
mov [6254h],bx;

ret
```
 ## Output  
 
![Screenshot (377)](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/db05d5bf-ecf7-4b62-93fe-78ab8235504e)

## Division alp 
```
org 100h

mov ax,0d545h;
mov bx,0a178h;
div bx;
mov [6935h],bx;

ret
```
## Output  
![Screenshot (376)](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/9af81cd9-7ba8-4b5d-a617-e8e9d0ce7ba8)
## Programs for logical operations:
### AND
```
org 100h
mov bx,1000h;
and bx,1111h;
mov [0040h+02],bx;
ret
```
![322804829-36e7da71-bc9b-4f6c-a8e7-8e7649a2c3f3](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/3b8cc2f3-8601-4597-86c5-fc05ecfdc5c5)
### OR:
```
org 100h
mov ax,[0040h+06];
mov bx,1000h;
or ax,bx;
mov [0040h+02],ax;
ret
```
![322805036-99e9f673-0e07-4ec4-bbc7-a2e05721dd31](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/010f6c3b-c24f-4ea3-8b75-3642ed53dc87)
### NOT:
```
org 100h
mov bx,0040h;
mov ax,[bx]; 
not al;
mov [0040h+04],ax;
ret
```
![322805176-14cd7db9-bd58-486b-b7d4-0d38a91a32d6](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/9c0950f7-c32c-438f-b87d-ccd3debe8b32)
### XOR:
```
org 100h
mov bx,0040h;
mov ax,[bx]; 
xor ax,bx;
mov [0040h+04],ax;
ret
```
![322805289-8e124a37-ef18-47f4-90fb-16cec9d02949](https://github.com/Kowsalyasathya/EXPERIMENT--01-ALP-FOR-8086/assets/118671457/c1163f7c-528f-4b6e-86ce-48fe1cc2d907)

## Result :
 
Hence ALP on fundamental arithmetic and logical operations is verified and executed.







