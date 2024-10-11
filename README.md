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
![Screenshot 2024-10-10 161738](https://github.com/user-attachments/assets/dc2cd49d-e8fb-469c-b9a4-8d3a1e11d4df)<br/><br/>

* First, we should learn about these terms=><br/>

-> RTL designs =><br/>
  * RTL means " Register Transfer Level ".
  * These are the designs programmed in RTL languages such as Verilog or VHDL.
  * It gives us software implementation of the hardware.<br/>
  
-> EDA tools =><br/>
  * EDA means " Electronic Design Automation ".
  * EDA tools are used to design and validate the semiconductor manufacturing process to ensure it delivers the required performance and density.
  * Used to design electronic systems in three key steps: simulation, design, and verification.
  * EDA tools allow teams to predict circuit behavior, assemble circuit elements, and anticipate chip performance.
  * Below are some EDA tools and processes in physical design.<br/><br/>
  ![Screenshot 2024-10-10 161942](https://github.com/user-attachments/assets/11e13109-ed9d-4fb4-9178-55522a3f2372)<br/><br/>


-> PDK data =>
  * PDK means " Process Design Kit ".
  * PDK is a set of files used within the semiconductor industry to model a fabrication process for the design tools used to design an integrated circuit.<br/>

## RTL to GDSII flow:
![Screenshot 2024-10-10 162205](https://github.com/user-attachments/assets/003a85da-5390-4f26-bf6c-1cc774da6e82)<br/><br/>
### 1.Synthesis:
-> It is the conversion of rtl program to a gate level netlist.<br/><br/>
![Screenshot 2024-10-10 162414](https://github.com/user-attachments/assets/737aa306-c5a7-4314-9451-14bd9a35116e)<br/><br/>
![Screenshot 2024-10-10 162513](https://github.com/user-attachments/assets/4cf1507d-dbb0-4720-8a9a-42b4376e37ee)<br/><br/>

### 2.Floor Planning and Power Planning:
-> Floor Planning is the process of allocating the area for different macros and cells on a die.<br/>
-> Power Planning is the process of providing power to macros and cells on a die.<br/><br/>
![Screenshot 2024-10-10 162938](https://github.com/user-attachments/assets/c05be72a-e893-45f8-bfa9-92bdecaec335)<br/><br/>
![Screenshot 2024-10-10 163001](https://github.com/user-attachments/assets/d11d9217-d80f-4c30-b894-3d3ec0383a63)<br/><br/>
![Screenshot 2024-10-10 163017](https://github.com/user-attachments/assets/fd53bef4-1c68-4993-9850-1c82eb388eca)<br/><br/>

### 3.Placement:
-> Placement is the process of placing the standard cells inside the core boundary in an optimal location.<br/>
-> There are two types of placements: Global and Detailed.<br/>
-> Global placement assigns general locations to movable objects, while detailed placement refines object locations to legal cell sites and enforces nonoverlapping constraints.<br/><br/>
![Screenshot 2024-10-10 163318](https://github.com/user-attachments/assets/6d04055f-22d9-48c1-ba1c-b4bbde14f32e)<br/><br/>

![Screenshot 2024-10-10 163353](https://github.com/user-attachments/assets/0a77f6e4-c21a-4233-88aa-9e851a590a1e)<br/><br/>

### 4.Clock Tree Synthesis(CTS):
-> Clock Tree Synthesis is a technique for distributing the clock equally among all sequential parts of a VLSI design.<br/><br/>
![Screenshot 2024-10-10 163735](https://github.com/user-attachments/assets/703cb0e0-2cfb-4e26-807a-0e759d630660)<br/><br/>
![Clock-network-topologies-A-Two-level-Y-Tree-B-Two-level-H-Tree-C-Two-level](https://github.com/user-attachments/assets/ed103222-4f21-4012-9e25-baf4b948237d)<br/><br/>

### 5.Routing:
->  Routing in the VLSI design course is making physical connections between signal pins using metal layers.<br/>
-> There are two types in routing : Global and Detailed.
![Screenshot 2024-10-10 164025](https://github.com/user-attachments/assets/4fa5b6b5-4e9f-43d5-b023-bb2d4634f571)<br/><br/>
![Screenshot 2024-10-10 164116](https://github.com/user-attachments/assets/93bb80d3-6f86-4ab2-857b-7f99b1fcf94c)<br/><br/>

### 6.Signoff:
-> Signoff is the process of verifying the design at final stage before going to the tape out.<br/><br/>
![Screenshot 2024-10-10 164302](https://github.com/user-attachments/assets/75b171ad-80bc-4ef1-a907-9f482756d38c)<br/><br/>

## Introduction to OpenLANE:
![Screenshot 2024-10-10 165611](https://github.com/user-attachments/assets/c3daca62-1d27-42bc-ae98-9b9ba281d6d4)<br/><br/>
-> OpenLane is an automated RTL to GDSII flow based on several components including OpenROAD, Yosys, Magic, Netgen, CVC, SPEF-Extractor, KLayout and a number of custom scripts for design exploration and optimization. The flow performs all ASIC implementation steps from RTL all the way down to GDSII.<br/><br/>
![Screenshot 2024-10-10 170433](https://github.com/user-attachments/assets/072db17e-9930-454d-9b4e-769be5e70143)<br/><br/>

### striVe SOC Family:
![Screenshot 2024-10-10 165840](https://github.com/user-attachments/assets/92a42190-72f9-4289-ad95-8d1f991560b7)<br/><br/>

### OpenLANE ASIC Flow:
![Screenshot 2024-10-10 170005](https://github.com/user-attachments/assets/8e6fde2e-9916-41dc-b6de-c023cbf6cdba)<br/><br/>
![Screenshot 2024-10-10 170031](https://github.com/user-attachments/assets/62e5a91c-ca33-45ff-ba3a-4a93b9182794)<br/><br/>
-> There are two modes of operation: Autonomous or Interactive<br/>
-> Design Space Configuration is used to find the best set of flow configurations.<br/><br/>
![Screenshot 2024-10-10 170327](https://github.com/user-attachments/assets/1877c90d-2e0a-4754-91d1-61202595b3ed)<br/><br/>
![Screenshot 2024-10-10 170407](https://github.com/user-attachments/assets/6918747d-ff04-4ca0-bf46-6d333efd53be)<br/><br/>

### DFT(Design For Testability):
-> We use " Fault " tool for DFT.<br/><br/>
![Screenshot 2024-10-10 170655](https://github.com/user-attachments/assets/d3637478-1ee3-487f-ad7b-42e0a007e2a1)<br/><br/>

### Physical Implementation:
-> We use " OpenROAD " for Physical Implementation.<br/><br/>
![Screenshot 2024-10-10 170824](https://github.com/user-attachments/assets/c23d1ffb-011d-406c-9f2c-943b14772794)<br/><br/>

### Logic Equivalence Checking(LEC):
-> We use Yosys for LEC.<br/><br/>
![Screenshot 2024-10-10 170948](https://github.com/user-attachments/assets/c97fb2a4-67f5-4f34-ac7c-963fb42b0a07)<br/><br/>

### Antenna Rules Violation:
![Screenshot 2024-10-10 171101](https://github.com/user-attachments/assets/60d8bd29-62dd-40a2-933c-3a50c18fe507)<br/><br/>
![Screenshot 2024-10-10 194534](https://github.com/user-attachments/assets/fdcc81b9-7cde-43f4-8dd5-b285c55a19c4)<br/><br/>
![Screenshot 2024-10-10 194619](https://github.com/user-attachments/assets/683a4f9a-462c-4a92-bb5f-5bbfa87e6562)<br/><br/>

### Static Timing Analysis:
-> Static timing analysis (STA) is a method of validating the timing performance of a design by checking all possible paths for timing violations.<br/>
-> OpenSTA is used for Static timing analysis.<br/><br/>
![Screenshot 2024-10-10 194700](https://github.com/user-attachments/assets/9185573b-1595-4626-ad1a-d331b8532432)<br/><br/>

### Physical Verification DRC & LVS:
-> Design Rule Checking (DRC) verifies as to whether a specific design meets the constraints imposed by the process technology to be used for its manufacturing.<br/>
-> Layout Versus Schematic (LVS) checking compares the extracted netlist from the layout to the original schematic netlist to determine if they match.<br/><br/>
![Screenshot 2024-10-10 194947](https://github.com/user-attachments/assets/cc33dd1a-c44f-4150-85c4-9cc01a23f1c2)<br/><br/>

## Implementation on EDA tools:
* Before going to the tools, we have to know some basic commands in Linux.
### cd:
* cd - Change Directory.
* To go to our work directory =>
> cd Desktop/<br/>
> cd work/<br/>
> cd tools/<br/>
> cd openlane_working_dir/<br/>
> cd openlane/<br/>

* We can also enter the command as=>
> cd Desktop/work/tools/openlane_working_dir/openlane<br/>

### ls:
* ls command line utility lists all the files and directories under a specified directory.
* There are many ways we can use ls.
* Three such ways are 'ls', 'ls -l', 'ls -ltr'.
* Below image will show difference in above commands.<br/><br/>
![VirtualBox_OpenLane_Ubuntu_Harshith_10_10_2024_20_43_33](https://github.com/user-attachments/assets/9f62260a-1b30-4b47-85b1-805a41aa9dc0)<br/><br/>
* We can see that 'ls' only shows file names. 'ls -l' shows file names with dates in alphabetical order.'ls -ltr' shows file names with dates in order of date of creation.<br/>

**Note** : To know about a command, we can use => " command_name --help".<br/>

### docker:
* To run bash, we are going to use command docker.
### pwd:
* pwd means "present working directory".
* It shows which directory we are working in.

* After opening bash, we have to enter
> ./flow.tcl -interactive
* It is used to run OpenLANE in Interactive mode 
* Now enter the below command
> package require openlane 0.9

### Design setup stage:
* We have to setup the filesystem specific to the flow.
* The location need to be setup for the flow to fetch.
* It will be done by following command
> prep -design picorv32a

* The syntax is that " prep -design design_name".The command will output this below.<br/><br/>
![OpenLANE](https://github.com/user-attachments/assets/73fd98a3-4f8d-4066-8549-39bcc03a1bda)<br/><br/>
* In "picorv32a" directory in "designs" directory, we can see that "runs" file will be created.


### Running Synthesis:
* The command to run the synthesis is
> run_synthesis

### Calculating the Flop ratio:
Flop Ratio = No. of D-Flip Flops/Total no. of cells <br/>
* D-flip flops are shown as "sky130_fd_sd_hd_dfxtp_2"
* Total No. of cells are shown as "Number of cells".
* See the below image for clarification.<br/><br/>
![Cells](https://github.com/user-attachments/assets/912cd433-819b-4eb5-9181-938c73c7e3e6)<br/><br/>
![dfx (3)](https://github.com/user-attachments/assets/05814de9-89c2-4a9c-ad15-55d1e786b2f5)<br/><br/>

* From this, flop ratio will be => 1613/14876 = 0.1084296853993009
* In percentage, it is equal to 10.84296853993009%


# Section - 2 : Good Floorplan vs Bad floorplan and Introduction to library cells
## 1. Defining Width and Height of core and die
### Utilization factor and aspect ratio:
* Utilization factor is the ratio of area occupied by the netlist to the total area of the core.
* Aspect ratio is the ratio of height to width of a cell.
**Note:** Don't be confused with MOSFET aspect ratio.<br/><br/>
![Screenshot 2024-10-11 151632](https://github.com/user-attachments/assets/09bc7724-2808-43bd-bfb4-4ecd4404bb4a)<br/><br/>

* let us consider all the cells shown in the above image have 1u. width and 1u. length each.
* Generally it looks like below image.<br/><br/>
![Screenshot 2024-10-11 152020](https://github.com/user-attachments/assets/cc80a5c0-02f1-447d-8a41-f2eadbd46ad9)<br/><br/>
* We are considering every shape to be a square of area 1 sq.units.
* So,the below images will show how we consider the area.<br/><br/>
![Screenshot 2024-10-11 151503](https://github.com/user-attachments/assets/662ca37e-a0fd-4cf9-adb6-c5b435a85d5d)<br/><br/>
![Screenshot 2024-10-11 151523](https://github.com/user-attachments/assets/4ee90733-56fe-4e42-896c-395623e41090)<br/><br/>
![Screenshot 2024-10-11 151609](https://github.com/user-attachments/assets/0561a027-610e-43ae-accb-fca2f96e6238)<br/><br/>

* Practically, utilization factor can't be 1. It is because there are many limititations to the design and many parasitic elements will be produced if the cells are side by side.And we disregarded interconnects,vias etc. in these images.
* Optimally, we take larger areas as shown below.<br/><br/>
![Screenshot 2024-10-11 152817](https://github.com/user-attachments/assets/fc5e5761-295d-4c45-9f56-17f69e78b42a)<br/><br/>

## 2.Define locations of preplaced cells:
![Screenshot 2024-10-11 153403](https://github.com/user-attachments/assets/7d262c43-c307-49c4-937a-aec7a5fe6d5f)<br/><br/>
* As the above image shows, we fist partition the who combination logic into pieces ( such as AOI or OAI logic ) and assign them in blocks such that the output of one block will be inputs to another block without changing functionality.
* Each  block will run separately.<br/><br/>
![Screenshot 2024-10-11 153703](https://github.com/user-attachments/assets/393a6959-12c9-449d-af4f-e29c6a0dda3f)<br/><br/>
![Screenshot 2024-10-11 153839](https://github.com/user-attachments/assets/cc4aa85b-2fe8-4b7a-91bb-5d4bb3d66a43)<br/><br/>
* We are going to consider each block as a black box.
* These single blocks will be separately created as IPs or modules and later will be instantiated in top module.
* It makes the blocks to be reused wherever they are required.
* Below is the image of some of the IPs.<br/><br/>
![Screenshot 2024-10-11 160132](https://github.com/user-attachments/assets/658a6d29-a556-47ca-84e2-b4c38251b6ba)<br/><br/>
* Below  is the picture of  preplaced cells.<br/><br/>
![Screenshot 2024-10-11 160506](https://github.com/user-attachments/assets/6c457b26-4ff5-4ebc-88b6-5cd38a0465a1)<br/><br/>
* They will be placed according to inputs and outputs.
* The position can't be changed.
* The height can't be changed for every cell but there each cell can have different widths.

## 3. Surrounding pre-placed cells with decoupling capacitors:
* As we considered before that there exists parasitic elements between cells, primarily the capacitance will be formed betwen interconnects,cells and other elements.
* So, we need to decouple the capacitor so that there will be no fringing fields and keep the signal integrity.
* Let us take below example.<br/><br/>
![Screenshot 2024-10-11 161122](https://github.com/user-attachments/assets/9e7dbc36-8bbd-40ca-be30-caf23b10208e)<br/><br/>
* There exists resistance and inductance due to length of the wire offers some impedance.
* There exists capacitance if there are crosstalks or if interconnects are near the substrate.
* MOS Capacitance exists in MOSFETs.
* These will cause power dissipation,delay and loss in signal integrity.<br/><br/>
![Screenshot 2024-10-11 161649](https://github.com/user-attachments/assets/f2c7e4b7-3600-4af9-a05d-0c52f8bb37b1)<br/><br/>
![Screenshot 2024-10-11 161759](https://github.com/user-attachments/assets/f6d7181d-310c-4409-afbd-a8772d5607d1)<br/><br/>
* Noise margin is an important factor which desides low voltage or high voltage.
* undefined zone is where the ouput is considerd "unknown".
* So, high noise margin is necessary.<br/><br/>
![Logic Level](https://github.com/user-attachments/assets/49fd4870-59bb-4398-bdc9-b38d6707f19c)<br/><br/>
* Now, we are going to add a decoupling capacitor. The voltage across this decoupling capacitor will be same as voltage supplied or slightly lower.<br/><br/>



























































