# NASSCOM_VSD_IAT_HARSHITH
# Section - 1: Inception of open-source EDA, OpenLANE and Sky130 PDK
### Packaging:
Below is an image of an arduino board.<br/><br/>
![Screenshot 2024-10-10 122614](https://github.com/user-attachments/assets/44a378ae-8bf8-4f1a-8bb8-937bbf2bb149)<br/><br/>
* We can see a chip was marked in yellow circle.Its block diagram is as shown below.<br/><br/>
![Screenshot 2024-10-11 172214](https://github.com/user-attachments/assets/f120bdfa-0dc6-479a-8b43-42bdb00b54bc)<br/><br/>

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
![Screenshot 2024-10-11 162449](https://github.com/user-attachments/assets/9c2e67ce-0469-4efe-80d0-fc240be28328)<br/><br/>
* The decoupling capacitor works according to the switching activity.
* If there is high switching activity, capacitor loses some charge and in low switching, capacitor replenishes the charge.<br/><br/>
![Screenshot 2024-10-11 164127](https://github.com/user-attachments/assets/e1bfb421-f937-4aeb-b687-f3bb6a2e5da7)<br/><br/>
* Decaps are decoupling capacitors from the image.

## 4.Power planning:
![Screenshot 2024-10-11 164447](https://github.com/user-attachments/assets/972f887d-08eb-490a-acb6-f5052a5caf4c)<br/><br/>
![Screenshot 2024-10-11 164749](https://github.com/user-attachments/assets/68f98592-8173-45a5-a973-2ce4a58d0742)<br/><br/>

* we can see in the image that blue line is a 16-bit wide bus and we are driving a signal from one cell to other (indicated by red line).
* Problem is with the signal integrity.
* We can't assure that the signal driven from one cell will reach other cell as same.
* This is a major factor affecting Digital Communication
* There might be losses or noises added or value changes.<br/><br/>
![Screenshot 2024-10-11 165014](https://github.com/user-attachments/assets/b867dd29-421b-4c61-8999-1045ecb201d3)<br/><br/>
* From above image, we can see that if capacitors are discharging at the same time, there will be ground bounce which causes values to go into unknown state. (due to noise margin).<br/><br/>
![Screenshot 2024-10-11 165324](https://github.com/user-attachments/assets/ac7db461-30ba-4c34-b84f-97d74fea5cda)<br/><br/>
* In this image, if all the capcitors which are not charged before going to charge at the same time, there will be drop in voltage.
* To solve these kinds of problems, we need to provide different levels of voltages or provide voltage in different geometries!.<br/><br/>
![Screenshot 2024-10-11 170837](https://github.com/user-attachments/assets/a8a83a2d-bc03-485a-8807-0fd7602f8bdc)<br/><br/>
![Screenshot 2024-10-11 171029](https://github.com/user-attachments/assets/f62dc25e-65ff-4342-bd7e-69c679684ffc)<br/><br/>

## 5.Pin Placement:
* Lets take two designs as shown below.<br/><br/>
![Screenshot 2024-10-11 171228](https://github.com/user-attachments/assets/e794facb-c70c-4811-aa0d-d0ebf302eed7)<br/><br/>
![Screenshot 2024-10-11 171314](https://github.com/user-attachments/assets/778765e4-db79-49f1-8115-12b2fea3f9bb)<br/><br/>
* By combining both the designs, it will look like this.<br/><br/>
![Screenshot 2024-10-11 171346](https://github.com/user-attachments/assets/e941b18d-ce7a-425d-bc07-e5fc7db13b56)<br/><br/>
* We an see that we have some common ports in both designs.Lets reduce them.<br/><br/>
![Screenshot 2024-10-11 171653](https://github.com/user-attachments/assets/fc881ae7-a0fb-4194-962f-57e4316368ce)<br/><br/>
* We can observe from both images that we tied clk1 and clk2 in both designs and it will reduce additional sources.<br/><br/>
![Screenshot 2024-10-11 172214](https://github.com/user-attachments/assets/49d1e1c4-6ef2-438a-bae2-e34acb80e762)<br/><br/>
* From this  image, we can see that clk1,clk2 and clkout have large pins than others because they are driving the signal to all cells and larger pins means less contact resistance.

## 6. Logic cell Placement Blockage:
* The pads location must not have any cells placed.
* If not programmed or trained correctly, automated tools may place the cells out of core area which is not a best thing.<br/><br/>
![Screenshot 2024-10-11 172826](https://github.com/user-attachments/assets/a541b621-c7d8-4241-bbba-cc518d89ade1)<br/><br/>

## Implementation of floorplan:
* Before running floorplan, we have run these steps.
> cd Desktop/work/tools/openlane_working_dir/openlane<br/>
> docker<br/>
> ./flow.tcl -interactive<br/>
> prep -design picorv32a<br/>
> run_synthesis<br/>

* After all these steps,now run the floor plan
> run_floorplan<br/>

* Below are the screenshots of starting and completion of floorplan.<br/><br/>
![run_floorplan](https://github.com/user-attachments/assets/191dfe43-6b12-47cc-be1e-44f25f5b7d07)<br/><br/>
![fp_success](https://github.com/user-attachments/assets/dfc032d7-db51-429e-bbc1-9fff85beb141)<br/><br/>

## Library binding and placement:
### 1.Binding netlist with phyical cells:
* The design we considered above forms a library as shown below.<br/><br/>
![Screenshot 2024-10-12 082123](https://github.com/user-attachments/assets/52471cab-a10b-4ec2-9255-8b2d3c480e83)<br/><br/>
* This library consists the information of cells such as functionality, delay and look up tables.
* The same library comes with different sizes to increase or decrease resistance and delay.Large size has less delay.<br/><br/>
 ![Screenshot 2024-10-12 082419](https://github.com/user-attachments/assets/f6f5536e-7f02-4178-970c-fac3a7b59da1)<br/><br/>

 ### 2.Placement:
 * We have place the particular netlist on the floorplan.<br/><br/>
 ![Screenshot 2024-10-12 082709](https://github.com/user-attachments/assets/ff706fce-e85d-4b2d-9760-eaed80b28ed0)<br/><br/>

 ### 3.Placement Optimization:
 * Problem arises when there is too long of distance between two cells as in the case of green cells.Here we have to use wire length estimation.<br/><br/>
 ![Screenshot 2024-10-12 083016](https://github.com/user-attachments/assets/dd8297c0-c1ac-46c9-9995-5b565070f921)<br/><br/>
 * First, we have to check which cells are distant to the input and output ports.
 * There, we have to insert the repeaters which are ' buffers '.
 * These buffers regenerate signal strength.
 * After placing bufffers to all cells, it looks like this.<br/><br/>
 ![Screenshot 2024-10-12 084242](https://github.com/user-attachments/assets/fd818594-5120-4698-8982-af4877081ad7)<br/><br/>
 * Here timing becomes the major problem.

## Library characterization and modelling:
* Here, we will see the design flow.<br/><br/>
![Screenshot 2024-10-12 084614](https://github.com/user-attachments/assets/cf21b4f9-510a-4578-bdb9-f60e939f9e49)<br/><br/>
![Screenshot 2024-10-12 084625](https://github.com/user-attachments/assets/b192438d-d5f0-480c-9fea-df62371e30d9)<br/><br/>
![Screenshot 2024-10-12 084637](https://github.com/user-attachments/assets/a99ad120-c5ef-46ff-a5a4-2c3f64c84c0c)<br/><br/>
![Screenshot 2024-10-12 084658](https://github.com/user-attachments/assets/404ab247-23bc-4429-9303-abc70ecbfc85)<br/><br/>
![Screenshot 2024-10-12 084718](https://github.com/user-attachments/assets/e9926763-bc1c-49d8-8ed7-1ffbe4fabedd)<br/><br/>
![Screenshot 2024-10-12 084739](https://github.com/user-attachments/assets/732ea851-dd5b-49bd-bf59-8f1de54a0413)<br/><br/>
* Static Timing Analysis is also known as Signoff Timing Analysis.

## Placement using OpenLANE:
* We know that there are two types of placements. Global and Detailed.
* Global placement main objective is to reduce the wirelength.
* We want to reduce " Half perimeter Wire Length (HPWL) " and converge the overflow.
* This is the result after " run_placement ".<br/><br/>
![run_placement (2)](https://github.com/user-attachments/assets/0c6b34a6-75d9-4f6c-bc44-537e3f2c62e4)<br/><br/>
![placed_zoom](https://github.com/user-attachments/assets/00c4cdbe-e164-4aaa-b23c-09f55dad867d)<br/><br/>
![placed](https://github.com/user-attachments/assets/3809d0e2-32c6-41a5-85e3-876306abda1e)<br/><br/>


## Cell Design Flow:
* In this task, we are going to see the flow of cell design.
* First, we are going to take a chip and point out the standard cells.<br/><br/>
![Screenshot 2024-10-12 095104](https://github.com/user-attachments/assets/1aeabfc3-2e71-4cc8-a79a-5ef676ac8ca1)<br/><br/>
![Screenshot 2024-10-12 095143](https://github.com/user-attachments/assets/657f45b8-8fa0-4489-97da-87ccfa15f731)<br/><br/>
* From the about image, " vt " means " Voltage Threshold ".
* HVT means " High Voltage Threshold ". These are used to save power. Only use where timing path is not critical.
* LVT means " Low Voltage Threshold ". These are used in timingcritical paths. These cells consume more power due to leakage.
* Other type of cells are ' SVT ' (Standard Voltage Threshold).Used for moderate power consumption and delay.Also called as RVT(Regular Voltage Threshold) cells.

## Designing an Inverter:
![Screenshot 2024-10-12 100205](https://github.com/user-attachments/assets/037f2bd8-275f-408f-a4b2-2b87e057b63f)<br/><br/>
* We have to design inverter using PDKs.
* We have to follow DRC (Design rule Check) and LVS (Layout vs Schematic).
* Based on these, we have to use lambda rules.<br/><br/>
![Screenshot 2024-10-12 100518](https://github.com/user-attachments/assets/09ac17f5-1ba8-4a17-9ef4-2f0c235c2db8)<br/><br/>
* SPICE models are used for parameter equations.<br/><br/>
![Screenshot 2024-10-12 100620](https://github.com/user-attachments/assets/fe7e05c9-aa8e-4e63-bbdb-1269f8f9878f)<br/><br/>
### User-defined Specifiations:
* Cell height and Cell width are user-defined.<br/>
-> Height must be same for all the cells.<br/>
-> Width can change to change the delay.<br/>
* Suppy voltage is another user-defined parameter.<br/>
-> The designer has to design the library cell such that those are within the noise margin levels.
* Metal layers.<br/>
-> There are many metal layers and designer have to choose metal layer according to width, type and contacts.
* Pin locations.<br/>
-> Change the location or direction of pins according to the requirement.
* Drawn gate length.<br/>
-> To increase or decrease the size of polysilicon gate.<br/><br/>
  ![Screenshot 2024-10-12 100850](https://github.com/user-attachments/assets/e5c201f8-e329-403d-88c5-3d507a506432)<br/><br/>
![Screenshot 2024-10-12 101055](https://github.com/user-attachments/assets/5b89468a-41c7-48b8-97bd-0d4f1bbb267e)<br/><br/>
![Screenshot 2024-10-12 101407](https://github.com/user-attachments/assets/414df5c4-0ed3-48e6-9d30-b62390f06f34)<br/><br/>
![Screenshot 2024-10-12 101531](https://github.com/user-attachments/assets/fbdd6855-3fd0-4962-a4f0-c1c0af8563b3)<br/><br/>
![Screenshot 2024-10-12 101601](https://github.com/user-attachments/assets/3f8fde07-46b0-437c-a040-85999c3c637f)<br/><br/>

## Design Steps:
### Circuit and Layout Design:
* First we have to implement the funtion.
* Next, we have to remove redundant terms inside the function.
* After function was implemented in CMOS or any other technology.
* Aspect ratio of PMOS and NMOS(if CMOS is being used) are to be designed.<br/><br/>
![Screenshot 2024-10-12 102013](https://github.com/user-attachments/assets/b3f89bb2-b8d2-4112-adca-3c2322482e20)<br/><br/>
### Characterization:
* Below is the layout of the buffer formed by cascading two inverters(NOT gates).<br/><br/>
![Screenshot 2024-10-12 102556](https://github.com/user-attachments/assets/c7162b5d-525f-4d50-a991-f8dfcd9b529d)<br/><br/>
![Screenshot 2024-10-12 102705](https://github.com/user-attachments/assets/64faad64-f10c-4b39-a385-fb46ca912528)<br/><br/>
* Below is the SPICE model of the circuit above. It contains circuit model, subcircuit models,technology models of PMOS and NMOS.<br/><br/>
![Screenshot 2024-10-12 102939](https://github.com/user-attachments/assets/eadc0c80-6cdb-4344-8f6d-f592e7b80a48)<br/><br/>
**Step-1**: We have to read the models and tech files of NMOS and PMOS.<br/>
**Step-2**: We have to read extracted SPICE netlist.<br/>
**Step-3**: Define how to recognize behaviour of the buffer.<br/>
**Step-4**: Read sub-circuit of the inverter.<br/>
**Step-5**: Attach necessary power sources.<br/>
**Step-6**: Application of stimulus.<br/>
**Step-7**: Apply necessarry output capacitances.<br/>
**Step-8**: Provide necessary simulation command.<br/><br/>
![Screenshot 2024-10-12 103808](https://github.com/user-attachments/assets/0449a81b-8364-45e2-ad77-ba361fd2fce5)<br/><br/>
![Screenshot 2024-10-12 103918](https://github.com/user-attachments/assets/ae88ec05-4550-4abf-98a6-e0cd876980c6)<br/><br/>

* Now, we have to provide all these characterizations to characterization software " GUNA ".
* GUNA will povide us with Timing,Noise and Power characterizations.<br/><br/>
![Screenshot 2024-10-12 104156](https://github.com/user-attachments/assets/fe73f8ff-e18f-4f54-a27f-e9e1b29b9fcd)<br/><br/>

## Timing Charcterizations:
* First, we need to know about "Slew Rate".
* Slew Rate is defined as ' the rate of change of signal's voltage over time '.
* Slew Rate = dV/dt (volts/sec).
* Optimum Slew Rate is " Infinite ".
* Practicaly, Slew Rate can't be infinite because of environment variables and nature of real-world objects.
* Below is an image of input and output of an inverter.Red line is input and blue line is output.<br/><br/>
![Screenshot 2024-10-12 104422](https://github.com/user-attachments/assets/087ef58b-d57e-4ef8-86a1-28d6f0b0d5ea)<br/><br/>
* We will see the images of each definition below.<br/><br/>
### slew_low_rise_thr:
* Typically the value is 20-30 % of voltage.<br/><br/>
![Screenshot 2024-10-12 105055](https://github.com/user-attachments/assets/5297bff3-18d6-42c0-a976-d59faf28ac0d)<br/><br/>
### slew_high_rise_thr:
* Typically the value is 80-90 % of voltage.<br/><br/>
![Screenshot 2024-10-12 105339](https://github.com/user-attachments/assets/92833caf-8dae-47de-9612-b243186205b5)<br/><br/>
### slew_high_fall_thr and slew_low_fall_thr:
* Similar to rise threshold.<br/><br/>
![Screenshot 2024-10-12 105516](https://github.com/user-attachments/assets/5ce07efe-4f93-4ea8-8bad-7a73586f1160)<br/><br/>
![Screenshot 2024-10-12 105527](https://github.com/user-attachments/assets/5f71db23-4694-4328-af61-b6fff78491f3)<br/><br/>

### In case of buffer:
### in_rise_thr:
* Typically at 50% of voltage value.<br/><br/>
![Screenshot 2024-10-12 105725](https://github.com/user-attachments/assets/ce16ab2d-91a6-430e-8302-8af63745c0b1)<br/><br/>
### in_fall_thr,out_rise_thr,out_fall_thr:
![Screenshot 2024-10-12 110429](https://github.com/user-attachments/assets/45336360-8158-4b02-bc33-7b4e7e92062e)<br/><br/>
![Screenshot 2024-10-12 110445](https://github.com/user-attachments/assets/a74228b0-cdf0-451d-846e-335837f97405)<br/><br/>
![Screenshot 2024-10-12 110453](https://github.com/user-attachments/assets/8ecffbe7-7221-4228-a192-eb427359509d)<br/><br/>

## Propogation Delay:
* Propogation delay is the time taken by the circuit to generate the output when input was given.
* Simply output_time - input_time.<br/><br/>
![Screenshot 2024-10-12 110809](https://github.com/user-attachments/assets/d7976df5-5a52-4a04-a2d6-30c54363feff)<br/><br/>
**Note** : Delay should not be negative.<br/><br/>

## Transition time:
* It is time taken for the pin to change its state i.e. transition from low to high or high to low.
* Typically we find difference between voltage at 10% and 90%.
* Depends on Slew Rate.<br/><br/>
![Screenshot 2024-10-12 111254](https://github.com/user-attachments/assets/0b1e1194-caaa-4421-b14b-77665182fb2d)<br/><br/>


# Section-3: Design library cell using Magic Layout and ngspice characterization
### VTC(Voltage Transfer Characteristics):
* we need to do following step as in the image.<br/><br/>
![Screenshot 2024-10-13 074853](https://github.com/user-attachments/assets/7de10807-9055-4887-9fa0-36b98174912d)<br/><br/>
![Screenshot 2024-10-13 075354](https://github.com/user-attachments/assets/924ae8d0-9e4a-4542-91e0-602b174186d4)<br/><br/>
* From above picture, all statements between " *** *** " are comments.
* Syntax for transistor description is  " Transistor_name drain_v gate_v source_v source_v transistor_type width length".
* We can observe that with changing the aspect ratios, the curve will change accordingly as shown below.<br/><br/>
![Screenshot 2024-10-13 080226](https://github.com/user-attachments/assets/9498dfc2-407b-4f4e-8612-778755ebc94d)<br/><br/>
![Screenshot 2024-10-13 075754](https://github.com/user-attachments/assets/82b72d74-286e-41f4-92b3-9f9349bab74b)<br/><br/>
* Now, we will see the robustness of a CMOS inverter. It retains the logic but changes the nature of curve according to the parameters.<br/><br/>
![Screenshot 2024-10-13 080833](https://github.com/user-attachments/assets/4dfc4d66-92c4-4cee-8b61-4232fe349ac5)<br/><br/>
* At switching threshold point, both NMOS and PMOS will be ON i.e in saturation region.<br/><br/>
![Screenshot 2024-10-13 080941](https://github.com/user-attachments/assets/61c3a635-0f1e-4ba8-b097-10d797746bda)<br/><br/>
* Calculation of vm:<br/><br/>
![Screenshot 2024-10-13 083055](https://github.com/user-attachments/assets/dc44473b-56e9-49ba-84d2-cd94ffae5890)<br/><br/>
* Now, we are gooing to experiment on different aspect ratios.
### Step-1:
* Retrieve the required files from github.
> git clone https://github.com/nickson-jose/vsdstdcelldesign.git<br/>
### Step-2:
* Copy sky130A techfile from magic to vsdstdcelldesign.
### Step-3:
* Give the following command.
> magic -T sky130A.tech sky130_inv.mag &
## CMOS Process:
![Screenshot 2024-10-13 091424](https://github.com/user-attachments/assets/ca73ad19-70df-4015-9efa-d9f931e94382)<br/><br/>
![Screenshot 2024-10-13 091443](https://github.com/user-attachments/assets/16237a05-f392-4bea-b379-1708c9161062)<br/><br/>
* Now, we are going to see how to process a CMOS.
### Steps:
* First, p-substrate will be taken(silicon wafer).
* A photoresist layer will be deposited.
* Now we have to protect one side with a mask.<br/><br/>
![Screenshot 2024-10-13 094019](https://github.com/user-attachments/assets/761a5434-e9d1-4ac7-b0de-7f7199423d89)<br/><br/>
![Screenshot 2024-10-13 094030](https://github.com/user-attachments/assets/02ce64ad-55ff-4fa6-9ea9-ce13fd745095)<br/><br/>
* Now, incident UV rays.Photoresist reacts to UV rays.(positive photoresist)
* Remove photoresist which was exposed .Etch the surrface.
* Remove the mask and implant Boron through ion implantation from high energy source.It creates a p-well.
* Same process for n-well too.Phosporous is used for n-well.(from high energy source).
* To diffuse the wells to half the substrate area, we have to put the wafers in the high temperature furnace.
* Now, to control the threshold of PMOS and NMOS, we are going to dope Boron to p-well and arsenic to n-well at low energy.<br/><br/>
![Screenshot 2024-10-13 095003](https://github.com/user-attachments/assets/bde71a1f-a2d5-4eed-9c7d-4fb59a8c5fe9)<br/><br/>
* Now, etch the original oxide using dilute Hydrogen flouride(HF) and regrow into high quality.
* Deposit polysilicon layer on top of the oxide.
* Now , implant arsenic or phosporous for low gate resistance.
* Now,put on the mask-6 as shown.<br/><br/>
![Screenshot 2024-10-13 095244](https://github.com/user-attachments/assets/7fed78bf-9e02-40a4-b450-6870fc818a75)<br/><br/>
![Screenshot 2024-10-13 095258](https://github.com/user-attachments/assets/9be020c2-0084-4b5e-8f43-0aa505aad490)<br/><br/>
* Now, incident UV rays and etch away polysilicon.Now,it looks like below image.<br/><br/>
![Screenshot 2024-10-13 095504](https://github.com/user-attachments/assets/320af9e3-58c5-479a-8ee8-19eef24f57e8)<br/><br/>
* We are now going to form Lightly Doped Drain(LDD).<br/><br/>
![Screenshot 2024-10-13 115530](https://github.com/user-attachments/assets/cebd8974-891e-42d3-acd7-8b5541ac2e4d)<br/><br/>
* P- and N- are used in LDDs. We require LDDs because of two reasons. => " Hot Electron Effect " and " Short Channel Effect ".
### Hot Electron Effect:
* It is caused when the size getting decreased but no change in Voltage levels which caused Electric Field(E=V/d) grow more strength.<br/><br/>
![Screenshot 2024-10-13 120007](https://github.com/user-attachments/assets/fa342e92-c88b-402b-8ccd-9f60f4c0f623)<br/><br/>
* If energy barrier crossed 3.2eV, the charge carriers will penetrate the oxide layer.
### Short Channel Effect:
* When channel length decreases Gate voltage can't control charge flow in channel and leakage current will be formed.
### Source and Drain formation:
* Now, do the same process to form gate and source terminals.Deposit SiO2 or Si3n4 layer and do plasma anisotropic etching and it wil leave side-wall spacers. <br/><br/>
![Screenshot 2024-10-13 120910](https://github.com/user-attachments/assets/176987bb-17f5-4994-b5d3-d9d9412e30a9)<br/><br/>
* Now, deposit thin layer of screen oxide to avoid channeling during implants.
* Again mask and implant and put the wafer in high temperature furnace to form source and drain<br/><br/>
![Screenshot 2024-10-13 122357](https://github.com/user-attachments/assets/d52e7f52-8a44-430e-9538-2560f05600c7)<br/><br/>
### Forming inteconnects and contacts:
* First, remove thin oxide using HF.
* Deposit Titanium on surface using " sputtering ".<br/><br/>
![Screenshot 2024-10-13 122631](https://github.com/user-attachments/assets/42b21d4a-b55c-4e45-b200-d0f692f2b32e)<br/><br/>
* Heat wafer with N2 at high temperature to get TiSi2 (low resistent) <br/><br/>
![Screenshot 2024-10-13 122819](https://github.com/user-attachments/assets/abfaca49-9274-44e7-a0f9-05f7015c29d6)<br/><br/>
* TiN also gets formed in the process.<br/><br/>
![Screenshot 2024-10-13 122906](https://github.com/user-attachments/assets/a7560ba1-f070-4ab8-9034-e069978cfca7)<br/><br/>
* Next, mask and etch TiN using RCA cleaning.<br/><br/>
![Screenshot 2024-10-13 123255](https://github.com/user-attachments/assets/b2c3b1fe-fe24-4ad8-8a91-e49fc46a826a)<br/><br/>
![Screenshot 2024-10-13 124445](https://github.com/user-attachments/assets/91dfee02-5cb4-4ebb-b50d-9e8210094981)<br/><br/>
### Higher level metal formation:
![Screenshot 2024-10-13 124610](https://github.com/user-attachments/assets/0412993b-00a9-417f-b3a9-43f9309793c9)<br/><br/>
![Screenshot 2024-10-13 124650](https://github.com/user-attachments/assets/0c993e1f-37bb-4b58-a429-460bafb9b486)<br/><br/>
![Screenshot 2024-10-13 124740](https://github.com/user-attachments/assets/e0289a3d-444f-4d5f-870f-4a5030377205)<br/><br/>
![Screenshot 2024-10-13 124815](https://github.com/user-attachments/assets/f22949a3-3bd4-4e23-b47e-3ab747a30062)<br/><br/>
![Screenshot 2024-10-13 124845](https://github.com/user-attachments/assets/bec5454f-6581-417a-bdef-2b2bf4176c28)<br/><br/>
![Screenshot 2024-10-13 125002](https://github.com/user-attachments/assets/aab6e085-0360-4e68-82dd-314f28279d44)<br/><br/>
![Screenshot 2024-10-13 125022](https://github.com/user-attachments/assets/ebebeec1-320d-4f70-b6ef-aa7806530342)<br/><br/>
![Screenshot 2024-10-13 125050](https://github.com/user-attachments/assets/dbf1963a-5b93-4e6e-8485-273aac680e7f)<br/><br/>
![Screenshot 2024-10-13 125121](https://github.com/user-attachments/assets/4d5a8016-0e92-445a-a2a9-33a2d7cf56db)<br/><br/>
![Screenshot 2024-10-13 125227](https://github.com/user-attachments/assets/90cc2534-6f43-4cb0-ae90-a791d3004ebd)<br/><br/>
![Screenshot 2024-10-13 125313](https://github.com/user-attachments/assets/f06d1df6-f51b-4c1e-8a84-0f4252273043)<br/><br/>

## Layout of inverter:
* To select a layer, press 's' and to select whole connections press 's' 2 times.
![inv_layout](https://github.com/user-attachments/assets/0ea41174-2730-4eb6-9b56-f2a9c83620ed)<br/>
* We are going to see the SPICE code for the circuit.For that, we have to use " ext2spice " command. <br/><br/>
![ext2spice](https://github.com/user-attachments/assets/6b40fbed-62e1-4e84-8fb7-aee276fba911)<br/><br/>
* Now, we are going to use our libraries.To edit press 'I'.
* Syntax for voltages is " Name Voltage_node_name node voltage_level ".
* For pulse signals " Name node_name Gnd PULSE(start_volt High_volt Start_time rise_time fall_time On_time Time_period). <br/><br/>
![waveforms](https://github.com/user-attachments/assets/dbb41844-7ccf-407c-8ad9-7af32bea097c)<br/><br/>
![cell_rise_delay](https://github.com/user-attachments/assets/fa6b2dc4-d122-4c3e-b3ef-2bc73908c401)<br/><br/>
![cell_fall-delay](https://github.com/user-attachments/assets/fe668aa4-3ff9-4439-b5ee-900b35901737)<br/><br/>
![perc50](https://github.com/user-attachments/assets/0a1aaabc-d208-475f-a2bb-f04d1a64ff1a)<br/><br/>
![ftd](https://github.com/user-attachments/assets/d0a1f5ae-4c68-4d8f-a53f-35da8b59adc6)<br/><br/>
![my_inv](https://github.com/user-attachments/assets/f7125c98-74ec-4143-a93c-d86d894754f1)<br/><br/>
* Rise time dealy (80% - 20%) = 4.08e-9 - 4.02e-9 = 60 ps.
* Fall time delay (20% - 80%) = 2.18e-9 - 2.12e-9 = 0.02e-9 = 20 ps.
* Cell rise delay = 4.05326e-9 - 4.05e-9 = 2.26 ps. 
* Cell fall delay (i/p - o/p (50%)) = 2.18656e-9 - 2.15e-9 = 36.56 ps.

### Rectifying problems in DRC section:
* Below is the link for "read the docs".<br/>
[https://skywater-pdk.readthedocs.io/en/main/rules/periphery.html](url)<br/>
* Below is the link for "opencircuit design".<br/>
[http://opencircuitdesign.com/magic/](url)<br/>
* Below is the link for "Google skywater-pdk".<br/>
[https://github.com/google/skywater-pdk](url)<br/>
* Now, we are going to download corrupted  skywater process magic tech files and work on them to rectify DRC errors.
* For that,we have to download some files.
* Follow the below steps.
* Go to home directory
> cd<br/>
* Download the files.
> wget http://opencircuitdesign.com/open_pdks/archive/drc_tests.tgz<br/>
* Extract the files
> tar xfz drc_tests.tgz<br/>
* Change directory into the lab folder
> cd drc_tests<br/>
* List all files
> ls -al<br/>
* view .magicrc file
> gvim .magicrc
* open magic tool in better graphics
> magic -d XR &<br/>
* Below is the screenshot.<br/><br/>
![run_cd](https://github.com/user-attachments/assets/f954b336-725d-4b47-9f3c-a818c140edaf)<br/><br/>
* Now, we are going to open " poly.mag " in " magic tool " or run command -> " load poly " in tkcon window.
* Now, we are going to load a tech file. in tkcon window, type
> tech load sky130A.tech<br/>
* To check DRC errors, we have to rerun DRC.
> drc check<br/>
* To check what error we got by "selecting" the incorrect cell.
> drc why<br/><br/>
![drc_why](https://github.com/user-attachments/assets/08206579-67f8-45ea-8482-0c84ca49ac70)<br/><br/>

































 







































































