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

* As shown in the image,we can see 'pads', 'core' , 'die'.<br/>
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
*  An ISA is an 'Abstract Interface' and called as " Architecture of computer'.
*  An ISA may be classified in a number of different ways.
*  A common classification is by architectural complexity.
*  A complex instruction set computer (CISC) has many specialized instructions, some of which may only be rarely used in practical programs.
*  A reduced instruction set computer (RISC) simplifies the processor by efficiently implementing only the instructions that are frequently used in programs, while the less common operations are implemented as subroutines, having their resulting additional processor execution time offset by infrequent use.
*  Mainly, an ISA is used to convey instructions to the hardware to implement a program.
*  Below images gives an example.<br/><br/>
![Screenshot 2024-10-10 141206](https://github.com/user-attachments/assets/2170043d-2bbd-40c0-8aaa-052250643550)<br/><br/>
![Screenshot 2024-10-10 141842](https://github.com/user-attachments/assets/3e20fb0e-b4a8-4eac-b9e5-89e914664df7)<br/><br/>
### Step-1:
We have written a c-program in an IDE.
### Step-2:
The compiler will turn the c-program into Assembly language Code.
Here it is RISC-V ISA.
This contains instructions written in binary or hexadecimal.
### Step-3:
This Assembly language code will be converted to machine code using assembler.
This machine language can be understood by hardware and it implements the program.<br/><br/>
![Screenshot 2024-10-10 142458](https://github.com/user-attachments/assets/3a8fc4ee-5859-4e0c-81e5-e765e8df1946)<br/><br/>

* Below image shows the flow of the process which was explained above.<br/><br/>

![Screenshot 2024-10-10 151847](https://github.com/user-attachments/assets/19965245-ddf3-49f6-bfbf-da315d4bb829)<br/><br/>

* Let us take stopwatch as an example.<br/><br/>
![Screenshot 2024-10-10 152109](https://github.com/user-attachments/assets/30c8b533-6143-4e11-a051-91e2f655350c)<br/><br/>

### How hardware will be interfaced:
* Hardware can only understand logic High or Low i.e. 0 or 1.<br/><br/>
![Screenshot 2024-10-10 152501](https://github.com/user-attachments/assets/1b047cb9-7a70-49b1-940e-d8d695fa0088)<br/><br/>

* Output of the assembly is a binary pattern.<br/><br/>
![Screenshot 2024-10-10 152754](https://github.com/user-attachments/assets/e4671a8b-f513-4609-9da4-d05b874db71d)<br/><br/>

* RTL understands the instructions and create a design.<br/><br/>
![Screenshot 2024-10-10 152855](https://github.com/user-attachments/assets/8b8a27c7-6ab3-4e5e-b6ef-a24bf3dc5b14)<br/><br/>

* RTL design will be synthesized into a netlist.<br/><br/>
![Screenshot 2024-10-10 153027](https://github.com/user-attachments/assets/31b9cb7a-3a0c-4a8c-8af2-7a4858abb708)<br/><br/>

* Hardware implementation of logic design happens through Physical Design.<br/><br/>
![Screenshot 2024-10-10 153121](https://github.com/user-attachments/assets/dcd12357-cd47-46f4-bf68-5aead923b3ac)<br/><br/>

## SOC Design Using Openlane:
A digital ASIC design process requires :<br/>
-> RTL Designs.<br/>
-> EDA tools.<br/>
-> PDK Data.<br/><br/>
![Screenshot 2024-10-10 153607](https://github.com/user-attachments/assets/cdadf75c-0d80-4479-82a6-c5622c1a6db0)<br/><br/>

* Below image shows some open-source tools and websites for the design.<br/><br/>
![Screenshot 2024-10-10 153823](https://github.com/user-attachments/assets/662ebdc6-f6f4-45ef-b0ff-34cd1508abf7)<br/><br/>

* First, we should learn about these terms=><br/>
-> RTL designs =><br/>
  * RTL means Register Transfer Level.
  * These are the designs programmed in RTL languages such as Verilog or VHDL.
  * It gives us software implementation of the hardware.<br/>
  
-> EDA tools =><br/>
  * EDA means Electronic Design Automation.
  * EDA tools are used to design and validate the semiconductor manufacturing process to ensure it delivers the required performance and density.
  * Used to design electronic systems in three key steps: simulation, design, and verification.
  * EDA tools allow teams to predict circuit behavior, assemble circuit elements, and anticipate chip performance.<br/>

-> PDK data =>
  * PDK means Process Design Kit.
  * PDK is a set of files used within the semiconductor industry to model a fabrication process for the design tools used to design an integrated circuit.<br/>



















