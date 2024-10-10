# NASSCOM_VSD_IAT_HARSHITH
# Section - 1: Inception of open-source EDA, OpenLANE and Sky130 PDK
### Packaging:
Below is an image of an arduino board.<br/><br/>
![Screenshot 2024-10-10 122614](https://github.com/user-attachments/assets/44a378ae-8bf8-4f1a-8bb8-937bbf2bb149)<br/><br/>
* We can see a chip was marked in yellow circle.Its block diagram is as shown below.<br/><br/>

![Screenshot 2024-10-10 122229](https://github.com/user-attachments/assets/fb50b3b5-ecc1-4e72-9815-4954224816d5)<br/><br/>

* The chip which was marked in yellow circle is the processor/SOC. Other are peripherals.<br/>
* But the misconception is that we consider whole chip as IC. But it is a 'package' and it looks as it is shown below. <br/><br/>

![Screenshot 2024-10-10 123227](https://github.com/user-attachments/assets/5a0deb51-b3c2-4fb2-8c72-ed6a516171ba)<br/><br/>

* It is a quad flat no-lead package.Some other types of packaging are shown below.<br/><br/>

![IC package](https://github.com/user-attachments/assets/950e3aa3-c6c8-47f3-aa14-b09da67d6632)<br/><br/>

From above image =><br/>
-> BGA : Ball Grid Array<br/>
-> DIP : Dual Inline Package<br/>
-> QFN : Quad Flat No-Lead Package<br/>
-> QFP : Quad Flat Package<br/>
-> SOP : Small-outline Package<br/>
-> SOT : small outline transistor<br/>

* The Ic will be sitting at the centre of the package(chip) and the chip is "Wire Bound" as shown in the below image.<br/><br/>
![Screenshot 2024-10-10 124137](https://github.com/user-attachments/assets/5401f254-1b6a-48a4-a9c1-49011c27a1a6)<br/><br/>

* Now, we are going to see inside the chip.<br/><br/>
![Screenshot 2024-10-10 124501](https://github.com/user-attachments/assets/dcf2f028-71ce-4125-9170-44b6c8b238d4)<br/><br/>

* As shown in the image,we can see 'pads', 'core' , 'die'.
-> PADS : These are used to complete interconnections between different chips or chip and the board.<br/>
-> Core : It is the area where the design exist.<br/>
-> Die  : It is the silicon wafer piece on which IC was fabricated.<br/>

* Below is an example of the chip we are discussing.<br/><br/>

![Screenshot 2024-10-10 125319](https://github.com/user-attachments/assets/e80aaa10-2c67-41ac-ac27-7f3e44e07bfc)<br/><br/>

### Foundry IPs:
![Screenshot 2024-10-10 125556](https://github.com/user-attachments/assets/fa634a2b-73bc-4a63-ac3a-f8fd848c7b65)<br/><br/>

* From above image, we can see some blocks that are mentioned as " Foundry IPs".<br/>
* IP means " Intellectual Property ".
* Foundry is the place where chips will be manufactured.Ex: TSMC,UMC etc.
* These IPs are foundry specific.
* Below image shows Macros.<br/><br/>

![Screenshot 2024-10-10 140714](https://github.com/user-attachments/assets/1ef47e24-bc28-4d2a-8c9d-35c2da38d38c)<br/><br/>

### Macros:
* Macros are small program or codes which can be reused.<br/><br/>

## Introduction to RISC-V ISA(Instruction Set Architecture):
*  An Instruction Set Architecture (ISA) is part of the abstract model of a computer that defines how the CPU is controlled by the software.
*  An ISA may be classified in a number of different ways.
*  A common classification is by architectural complexity.
*  A complex instruction set computer (CISC) has many specialized instructions, some of which may only be rarely used in practical programs.
*  A reduced instruction set computer (RISC) simplifies the processor by efficiently implementing only the instructions that are frequently used in programs, while the less common operations are implemented as subroutines, having their resulting additional processor execution time offset by infrequent use.
*  Mainly, an ISA is used to convey instructions to the hardware to implement a program.






