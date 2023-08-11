# ASIC Theory
ASIC stands for Application-Specific Integrated Circuit. It is a type of integrated circuit (IC) that is specially designed for a particular application or use case rather than being a general-purpose chip. ASICs are optimized for specific tasks, and their design is tailored to perform those tasks efficiently and with high performance.

The Github repository documents and tracks the progress for the course Physical Design ASIC(VL508).  



## DAY 0 - Installation

<details>
<summary> <strong> Yosys </strong> - Open-Source RTL Synthesis Tool </summary>

Yosys is a powerful and widely-used open-source RTL synthesis tool that enables designers to convert Verilog RTL code into optimized gate-level representations suitable for ASIC or FPGA implementation. It is designed for digital hardware design and offers a plethora of features, including RTL synthesis, technology mapping, optimization, and formal verification capabilities. With a scripting interface and an active community of users and developers, Yosys provides flexibility, efficiency, and cost-effectiveness for various digital design projects.

**Key Features**:
- RTL Synthesis: Yosys takes Verilog RTL code as input and performs RTL synthesis, generating a gate-level netlist.
- Technology Mapping: The tool maps the RTL design to a specific library of standard cells, allowing optimization for target technologies.
- Optimization: Yosys employs various algorithms to optimize the design for improved performance, area, and power consumption.
- Formal Verification: The tool includes formal verification capabilities to ensure the correctness of the design.
- Scripting Interface: Yosys provides a scripting interface, enabling users to write custom synthesis scripts for specific design flows and optimizations.
- Open-Source and Community-Driven: Yosys is an open-source project with an active community, constantly contributing to its development and improvement.
  
**Installation**

Yosys is installed using the following set of steps.

```bash
$ git clone https://github.com/YosysHQ/yosys.git
$ cd yosys-master 
$ sudo apt install make (If make is not installed please install it) 
$ sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
$ make config-gcc
$ make 
$ sudo make install
```
Screenshot after installation-
![yosys](https://github.com/Shant1R/Shant_IIITB/assets/59409568/6ac97051-4660-4722-b384-26eb6aba3260)

</details>

<details>

<summary><strong>Icarus verilog</strong> - Open-Source Verilog Simulation and Synthesis Tool</summary>

Iverilog is a widely-used open-source Verilog simulation and synthesis tool that allows designers to simulate and synthesize digital hardware designs described in Verilog HDL. It offers a comprehensive set of features for both simulation and synthesis, making it a valuable tool for digital design projects of all scales. With its versatility and community-driven development, Iverilog provides an efficient and cost-effective solution for verifying and implementing digital designs.

**Key Features**:
- Verilog Simulation: Iverilog supports simulation of Verilog designs, enabling users to test and verify their digital circuits' functionality.
- Synthesis Support: The tool provides synthesis capabilities, allowing designers to generate gate-level netlists suitable for ASIC or FPGA implementation.
- IEEE Standard Compliance: Iverilog adheres to the IEEE 1364-2005 Verilog standard, ensuring compatibility with a wide range of Verilog designs.
- VPI (Verilog Programming Interface) Support: Iverilog supports VPI, enabling users to write C/C++ programs to interact with the simulation or synthesis process.
- Efficient and Scalable: Iverilog is known for its efficiency, making it suitable for small hobbyist projects as well as large-scale commercial designs.
- Open-Source and Community-Driven: Being an open-source tool, Iverilog benefits from an active community of users and developers, continually improving and enhancing its capabilities.
  
**Installation**

Icarus Verilog also known as iverilog is installed using the following command.

```bash
$ sudo apt-get update
$ sudo apt-get install iverilog

```
Screenshot after installation-
![iverilog](https://github.com/Shant1R/Shant_IIITB/assets/59409568/4f77ee22-b0b3-4c96-9f8e-1b74443579e4)


</details>

<details>
<summary><strong>GTKWave</strong> - Open-Source Waveform Viewer for Digital Simulation</summary>

GTKWave is a popular open-source waveform viewer designed to visualize and analyze simulation results of digital designs. As an essential tool in digital hardware development, GTKWave allows users to examine waveforms generated by Verilog or VHDL simulation, making it easier to debug and verify the behavior of complex digital circuits. With its user-friendly interface and active community support, GTKWave is a valuable asset for engineers and hobbyists involved in digital design and verification projects.

**Key Features**:
- Waveform Visualization: GTKWave provides a graphical interface to display simulation waveforms, helping users gain insights into the behavior of digital circuits.
- Support for Various Formats: The tool supports various waveform formats, including VCD (Value Change Dump), FST (Fast Signal Trace), LXT, and VZT.
- Zoom and Navigation: GTKWave allows users to zoom in and out on specific regions of the waveform and provides convenient navigation tools for easy waveform analysis.
- Signal Grouping: Users can group related signals together, simplifying the visualization of complex designs.
- Cross-Platform Compatibility: GTKWave is available for multiple platforms, including Windows, macOS, and Linux, making it accessible to a wide range of users.
- Extensible and Customizable: Users can extend GTKWave's functionality through scripting and customize the appearance and behavior of the waveform viewer.
- Open-Source and Community-Driven: As an open-source project, GTKWave benefits from continuous community contributions, ensuring the tool's ongoing improvement and relevance

**Installation**

GTKWave is installed using the following commands.

```bash
$ sudo apt update
$ sudo apt install gtkwave
```
Screenshot after installation-
![gtkwave](https://github.com/Shant1R/Shant_IIITB/assets/59409568/ae8c7922-c337-4157-839f-c8f1f62265b2)

</details>


<details>
<summary><strong>OpenSTA</strong> - Open-Source Static Timing Analysis Tool</summary>

OpenSTA is a powerful open-source Static Timing Analysis (STA) tool designed to analyze digital integrated circuits and provide critical timing information. As an essential component of the digital design flow, OpenSTA enables engineers to perform timing verification, identify potential timing violations, and optimize the performance of complex designs. With its versatile features and community-driven development, OpenSTA is a valuable resource for designers working on ASIC or FPGA projects.

**Key Features**:
- Static Timing Analysis: OpenSTA performs static timing analysis to determine the critical paths and timing violations in digital designs.
- Liberty File Support: The tool supports industry-standard Liberty format files, which contain timing information about the standard cells used in the design.
- Path Tracing and Reporting: OpenSTA traces critical timing paths and generates detailed timing reports, highlighting setup and hold violations.
- Constraints Support: Designers can specify timing constraints in the design using standard Synopsys Design Constraints (SDC) files, which OpenSTA interprets during the analysis.
- Highly Scalable: OpenSTA can handle designs of varying sizes, from small digital circuits to large-scale industrial projects, making it suitable for a broad range of applications.
- Interactive Visualization: OpenSTA provides an interactive graphical interface to visualize and navigate through the timing paths in the design.
- Open-Source and Community-Driven: As an open-source project, OpenSTA benefits from contributions and feedback from a community of users and developers, ensuring continuous improvement and adaptability to new technologies.

**Installation**

To install OpenSTA, follow the given github link and download the following prerequisites- 

```bash
https://github.com/The-OpenROAD-Project/OpenSTA
```

```bash
$ sudo apt-get install cmake
$ sudo apt-get install clang
$ sudo apt-get install gcc
$ sudo apt-get install tcl
$ sudo apt-get install swig
$ sudo apt-get install bison
$ sudo apt-get install flex
```

Installation commands for openSTA
```bash
$ git clone https://github.com/The-OpenROAD-Project/OpenSTA.git
$ cd OpenSTA
$ mkdir build
$ cd build
$ cmake ..
$ make
```
Screenshot after installation-
![opensta](https://github.com/Shant1R/Shant_IIITB/assets/59409568/36537253-8d3e-4f7a-9358-35c3f5c04e55)

</details>


<details>
<summary><strong>NGSpice</strong> - Open-Source Circuit Simulation Tool</summary>

Ngspice is a powerful open-source circuit simulation tool that allows engineers, researchers, and hobbyists to analyze and simulate electronic circuits. As a widely-used circuit simulator, Ngspice can handle analog, digital, and mixed-signal circuits, providing valuable insights into circuit behavior, performance, and characteristics. With its extensive set of features and active community support, Ngspice serves as an essential tool for circuit design, analysis, and optimization.

**Key Features**:
- Mixed-Signal Simulation: Ngspice supports mixed-signal simulation, enabling the analysis of circuits containing both analog and digital components.
- Circuit Modeling: The tool supports a wide range of device models, including passive components, diodes, transistors, operational amplifiers, and more.
- Advanced Analysis: Ngspice provides various analysis types, such as DC, AC, transient, and noise analysis, allowing users to evaluate circuit performance under different conditions.
- Extensibility: Users can add custom models, algorithms, and simulation capabilities through scripting and user-defined subcircuits.
- SPICE Compatibility: Ngspice adheres to the SPICE (Simulation Program with Integrated Circuit Emphasis) standard, ensuring compatibility with existing SPICE netlists.
- Cross-Platform Support: Ngspice is compatible with multiple operating systems, including Windows, macOS, and Linux, making it accessible to a broad user base.
- Open-Source and Community-Driven: Being an open-source project, Ngspice benefits from active community contributions, bug fixes, and enhancements, ensuring its continuous development and reliability.

**Installation**

NGSpice is installed using the following commands.

After downloading the tarball from https://sourceforge.net/projects/ngspice/files/ to a local directory, unpack it using:

```bash
$ tar -zxvf ngspice-37.tar.gz
$ cd ngspice-37
$ mkdir release
$ cd release
$ ../configure  --with-x --with-readline=yes --disable-debug
$ make
$ sudo make install
```
Screenshot after installation-
![ngspice](https://github.com/Shant1R/Shant_IIITB/assets/59409568/726fcc95-63eb-4089-87e3-f306cc37d83c)

    
</details>

<details>
<summary><strong>Magic</strong> - Open-Source VLSI Layout and Chip Design Tool</summary>
Magic is a widely-used open-source VLSI (Very-Large-Scale Integration) layout and chip design tool. It offers a versatile and user-friendly environment for designing, editing, and analyzing integrated circuit layouts. As an essential tool in the physical design flow, Magic allows engineers and researchers to create complex IC layouts and verify their correctness before fabrication. With a range of features and active community support, Magic is a valuable asset for digital and analog chip designers and hobbyists.

**Key Features**:
- Layout Editing: Magic provides an intuitive interface for designing and editing integrated circuit layouts, enabling efficient placement and routing of various circuit elements.
- Custom Design Rules: Users can define custom design rules, allowing them to tailor the layout to specific technology nodes and manufacturing processes.
- Hierarchical Design: Magic supports hierarchical design methodologies, enabling the creation of complex designs by organizing circuits into hierarchical blocks.
- Design Rule Checking (DRC): The tool performs design rule checks to identify potential layout errors and violations before the chip fabrication process.
- Extraction and Simulation: Magic allows extraction of parasitic components and supports SPICE netlist simulation for accurate performance evaluation.
- Scripting and Automation: Users can extend Magic's functionality using scripts, automating repetitive tasks and customizing the design flow.
- Cross-Platform Support: Magic is compatible with various operating systems, including Windows, macOS, and Linux, making it accessible to a wide range of users.
- Open-Source and Community-Driven: As an open-source project, Magic benefits from an active community of users and developers, ensuring continuous improvement and adaptability to new design challenges.

**Installation**
  
Magic is installed using the following commands.

```bash
$   sudo apt-get install m4
$   sudo apt-get install tcsh
$   sudo apt-get install csh
$   sudo apt-get install libx11-dev
$   sudo apt-get install tcl-dev tk-dev
$   sudo apt-get install libcairo2-dev
$   sudo apt-get install mesa-common-dev libglu1-mesa-dev
$   sudo apt-get install libncurses-dev
$   git clone https://github.com/RTimothyEdwards/magic
$   cd magic
$   ./configure
$   make
$   sudo make install

```
Screenshot after installation-
![magic](https://github.com/Shant1R/Shant_IIITB/assets/59409568/f5fe09ee-2f15-47c0-b4a6-5a41febf7e76)
    
</details>

<details>
<summary><strong>OpenLANE</strong>- Open-Source Digital ASIC Design Flow</summary>

OpenLane is a comprehensive open-source digital ASIC (Application-Specific Integrated Circuit) design flow that facilitates the design and implementation of complex digital chips. It provides a complete RTL-to-GDSII (RTL to Graphic Design System II) flow, encompassing synthesis, placement, routing, and manufacturing processes. OpenLane streamlines the ASIC design process and enables designers to create custom digital chips with greater efficiency and accessibility. With an extensive set of features and community support, OpenLane is a valuable tool for ASIC designers, researchers, and hobbyists alike.

**Key Features**:
- RTL-to-GDSII Flow: OpenLane offers an end-to-end design flow, starting from RTL synthesis to final GDSII layout generation, ensuring a seamless ASIC design process.
- Synthesis and Optimization: The tool performs RTL synthesis and optimization to generate an efficient gate-level representation of the design.
- Placement and Routing: OpenLane optimizes chip placement and performs routing to connect all the components efficiently.
- DRC and LVS Checks: OpenLane includes design rule checking (DRC) and layout versus schematic (LVS) checks to ensure the design's manufacturability and correctness.
- PDK Integration: The tool integrates with Process Design Kits (PDKs) from various foundries, supporting a wide range of technology nodes and manufacturing processes.
- Scripting and Customization: Users can write scripts to customize various aspects of the design flow and automate repetitive tasks.
- Performance and Area Optimization: OpenLane offers options to optimize the design for performance, area, or power based on the project's requirements.
- Cross-Platform Support: OpenLane is compatible with multiple operating systems, including Windows, macOS, and Linux, making it accessible to diverse design teams.
- Open-Source and Community-Driven: Being an open-source project, OpenLane benefits from continuous community contributions, bug fixes, and enhancements, ensuring its continuous development and improvement.

**Installation**

OpenLane is installed using the following commands.

```bash
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt install -y build-essential python3 python3-venv python3-pip make git
$ sudo apt install apt-transport-https ca-certificates curl software-properties-common
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
$ echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
$ sudo apt update
$ sudo apt install docker-ce docker-ce-cli containerd.io
$ sudo docker run hello-world
$ sudo groupadd docker
$ sudo usermod -aG docker $USER
$ sudo reboot 
```

After Reboot
```bash
$ docker run hello-world
```

```bash
$ cd $HOME
$ git clone https://github.com/The-OpenROAD-Project/OpenLane
$ cd OpenLane
$ make
$ make test
```

Screenshot after installation-
![openlane](https://github.com/Shant1R/Shant_IIITB/assets/59409568/d55be32a-a662-4284-94b0-b0d53af2fbca)

</details>

## DAY 1 - Introduction to Verilog RTL design and Synthesis

<details>
<summary><strong>Open Source simulator iverilog</strong></summary>

Simulator is a tool to verify that the said design adheres to the functionality to its intended specifications. It works by following the input given and changes the output accordingly, thus one can compare the desired output and the output derived for the said inputs.

Simulator architecture schematic diagram -
![Simulator](https://github.com/Shant1R/Shant_IIITB/assets/59409568/11d0647f-499b-4ea9-ab80-8c6ef20da093)

Under the given repository, **Iverilog** is used which is an open source simulator.
- Design is the set of verilog codes with the aim to create a functionality that meets the given specifications. 
- Testbench is the set of code which provides the stimulas or test vectors to the desgin under test to verify the design working.
- It is to be noted multiple inputs can be given the design block and multiple outputs can be derived.
- The testbench is not given any external inputs. Testvectors are given under the testbench itself.
- The output of the simulator is a VCD file, ie. value change dump file which is viewed using **GTKWave** to visualise the waveform.

Simulation flow of Iverilog - 
![workflow](https://github.com/Shant1R/Shant_IIITB/assets/59409568/b67eb2d2-478e-4745-9876-7846de6a01c0)

</details>


<details>
<summary><strong>Introduction to Lab</strong></summary>

Under this, we will go through how to setup the directory and lab for the course and how to access various files and execute.

**Lab Setup**

The first step under the lab setup for the course is to form a seperate directory as VLSI and git clone the course files from the given repository in the code.



```bash
$ cd Documents
$ cd ASICs
$ cd VLSI
$ cd git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git
```

Terminal Window - 
![sky130_gitclone](https://github.com/Shant1R/Shant_IIITB/assets/59409568/8e74128d-3341-4378-9c40-309260327bef)

Upon the cloning, a new folder with the name *sky130RTLDesignAndSynthesisWorkshop* is made. Under this folder, there will be several folders, such as lib which contains the standard set library for sky130 which will be used for the synthesis, verilog_files which contains all the source files and testbenches for the experiments to be done. The contents of each folder can be seen by going into the directory and entering ls.


**Working with iverilog and gtkwave - MUX**

Under this, we go over how load files on iverilog and visualise using gtkwave. The terminal is opened and the directory is set to the verilog_files, where various source files and their respective testbenches are stored. Under this example we will execute the mux using good_mux.v and check the functionality using gtkwave to visualise the dumpfile generated. Both the source file and testbench are loaded to iverilog. 

```bash
$ cd VLSI
$ cd sky130RTLDesignAndSynthesisWorkshop
$ cd verilog_files/
$ ls
$ iverilog good_mux.v tb_good_mux.v
$ ./a.out
$ gtkwave tb_good_mux.vcd
```

Screenshot of the terminal - 
![good_mux_terminal](https://github.com/Shant1R/Shant_IIITB/assets/59409568/06396f49-0e6c-487b-8408-82491557a852)

Waveform on GTKWave - 
![good_mux_gtk](https://github.com/Shant1R/Shant_IIITB/assets/59409568/cc8ec616-ac4d-4bc1-801f-0e680247ad69)

The waveform on gtkwave is used to check the variations in the output with the input.

**Code Explaination - MUX**

To edit the code, one can directly open the files or use gvim. The code to access both the source and testbech is given

```bash
$ gvim tb_good_mux.v -o good_mux.v
```


Editor window - 
![code_good_mux](https://github.com/Shant1R/Shant_IIITB/assets/59409568/cf8ca326-755a-4664-ae0b-8c01b8e94723)

There can be multiple ways to generate a mux. Under the given source code. it checks for the select line, if sel is 1, the output follows the input line 1 else it follows input line 0. Under the testbench, the inputs are set as reg and output as wire. The testbench has no primary inputs like the design source code. It instantiate the source code as uut - unit under test, any name can be used. Under the testbench, the dumpfile is generated for visualisation. The input variables are set and the toggled periodically and sets an end time. 

</details>


<details>
<summary><strong>Introduction to Yosys and Logic synthesis</strong></summary>

The RTL design is the behavioural model of the said specification written in an HDL language. For mapping this code to a hardware circuit comes the synthesis. The RTL code is translated to gate level using the front end libraries that are .lib files, through synthesis the netlist file is derived. 

The front end library is also called .lib, which can be explained as a collection for modules for the logic gates for the mapping. It contains various types of the same logic gate, such as 2 and 3 input and gates, and modules for the same gate with different execution speed, which can de decided upon the usecase and required specification. The speed of the gates depends the load, which for digital circuits are capacitors, thus charging and discharging of capacitors determine the speed of the gate, thus the system. For faster speed, we need transistor with more current sourcing capacity. Thus the need for wider transistors. But wider transistors enables faster processes with the trade off of power and area. Narrow transistors comsumes lesser area and power, but comes with bigger delays. Thus the choice of the gate models is made accordingly. The time delat should small enough to cover the propogation delay and setup times and at the same time large enough that it doesn't cause a hold crisis, that is its bigger than the hold time of the next gate in process.


One has to guide the synthesizer for the required execution time, ie, the use of faster and slower transistor models while mapping. This is known as constraints.    

The synthesizer used under this coursework is Yosys. 

Yosys setup flow-
![yosys1](https://github.com/Shant1R/Shant_IIITB/assets/59409568/35698376-e603-40eb-b5a4-a84965620587)

The design block has the function read_design and .lib  has a read_liberty function which reads the design file and .lib respectively. The netlist block has the fucntion read_netlist which upon execution generates the netlist file for the given design. It is to note design file and netlist file are two different representations for the same given specification.  

Synthesis verification flow - 
![yosys2](https://github.com/Shant1R/Shant_IIITB/assets/59409568/8c89fc9e-7d6a-426e-b55f-3927db75d7e7)

To verify the synthesis output, we use the iverilog simulator which is given the netlist and testbench as inputs, attain a vcd file, which is visualised using gtkwave. The output on the gtkwave with the netlist file should be the same as in the case of RTL simulation. Since the primary inputs and outputs in case of RTL designs and netlist design remains the same, the same testbench can be used to verify the design. 


</details>



<details>
<summary><strong>Lab using Yosys and Sky130 PDKs</strong></summary>

Under this section, we go through how to invoke the synthesizer yosys and synthesize the design. For the demonstration, we have taken the synthesis of mux, the good_mux.v file, which we have previously simulated before. 

- Step one is to go to the directory for the verilog files and invoke yosys synthesizer.

```bash
$ cd Documents/ASICs/VLSI/sky130RTLDesignAndSynthesisWorkshop/verilog_files/
$ yosys
```

![yosys_lab_1](https://github.com/Shant1R/Shant_IIITB/assets/59409568/24e98dd7-b81c-4398-a0cb-f5d5bf872813)

- Now we read the .lib using *read_liberty* and the path is set to the .lib files.
- The behavourial model of mux is read using *read_verilog* followed by determining the module name to be synthesized.
- The netlist is generated by *abc -liberty* followed by the path to .lib which specifies what gates are to be linked. Thus the RTL file is converted to netlist.
- The logic being realised can be view using *show*.

```bash
 read_liberty -lib ~/Documents/ASICs/VLSI/sky130RTLDesignAndSynthesisWorkshop/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
 read_verilog good_mux.v
 synth -top good_mux
 abc -liberty ~/Documents/ASICs/VLSI/sky130RTLDesignAndSynthesisWorkshop/verilog_files/sky130_fd_sc_hd__tt_025C_1v80.lib
 show
```

![yosys_lab_2](https://github.com/Shant1R/Shant_IIITB/assets/59409568/e3861c1c-4493-4fe1-822b-7e5179d95ab0)

- The netlist file is wriiten using *write_verilog* followed by the name for the file.
- Gvim edittor is used view the netlist file.

```bash
 read_verilog good_mux_netlist.v
 !gvim good_mux_netlist.v  
```

![yosys_lab_3](https://github.com/Shant1R/Shant_IIITB/assets/59409568/c201daec-bc2b-44f7-83c5-77ab3dd37e9d)

- It can seen that the netlist file has extra informations, thus to generate a simple netlist file we add an extra switch.
- After *write _verilog* we add *-noattr* before the file name.
- We attain a simpler netlist representation for mux.

```bash
 read_verilog -noattr good_mux_netlist.v
 !gvim good_mux_netlist.v
```

![yosys_lab_4](https://github.com/Shant1R/Shant_IIITB/assets/59409568/a917b533-9932-46bd-adfb-032cea61855b)

  
</details>

## DAY 2 - Timing libs, Hierarchical vs Flat synthesis and effective flop coding styles

<details>

<summary><strong>Introduction to .lib</strong></summary>
Under this section, we get a better insight regarding .lib. We have the general overview that it stores the models of all the standards cells, various variations and flavours as per the need of specification provided. Getting an insight into the .lib file, we start with the file name -  

*sky130_fd_sc_hd__tt_025C_1v80*

The name sky130 represemts that the library is based on 130nm technology. Under the nomenclature, we define PVT - process, voltage and temperature. Process refers to the variations due to the fabrication, ie. there will variations in the silicon fabricated even by the same machine. There is variation due to the voltage and temperature as well. Silicon is very sensitive to temperature. All these 3 determines how the silicon is going to perform. We aim to design such that silicon works in all the conditions, across various variations. These three are indicated under the name, tt stands for typical process, 25c indicates the temperature - 25C and 1v80 indicates the voltage of 1.80volts.  It is to be noted, all the models under the said library are designed for the given PVT parameters.

We open the .lib file using gvim to go through various other informations it provides.

![lib_1](https://github.com/Shant1R/Shant_IIITB/assets/59409568/f1a46b64-c496-4fd4-82e7-ef43e091964b)

- It defines the technology begin used "CMOS" and the delay model as "table_lookup"
- it defines the units for various parameters and quanities, such as, 1ns for time, 1V for voltage, 1mA for current, 1kohm for resistance and 1pF for capacitance.
- It defines the operating conditions as "tt_025C_1v80".

We take an example for a cell to understand the contents. Taking the example of a21110i cell. 

![lib_2](https://github.com/Shant1R/Shant_IIITB/assets/59409568/9996a4bc-1328-4436-91f0-551a17dd7d72)

- The given cell executes the logic for 5 inputs, *and* for the first two inputs and *or* it with the next three inputs, finally *not* the final expression.
- Logic implemented --> !((A1&A2)|B1|C1|D1)
- Since we got 5 inputs, there are 32 possible outputs. The .lib file contains the power consumption and timing details for all the possibilities.


Considering a two input *and* gate, and compare different two input and gate.

![lib_3](https://github.com/Shant1R/Shant_IIITB/assets/59409568/717b8741-8d21-413e-95b2-968c38eef551)

- The lib files conatins the power and timing information for the 4 possible outcomes.
- All three taken cells are 2 input and gates, but differ in their areas, and2_4 has a larger area than area2_2 and consequently more than and2_0.
- Having a larger area refers to the use of a wider cell. Wider cells will be faster, but consumes more power. This can be seen in the datials under the lib file.


  
</details>


<details>

<summary><strong>Heirarchial vs Flat Synthesis</strong></summary>

Under this section, we take the case of multiple_modul2s.v from verilog files to have a better unstanding.
```bash
  shant@shant:~/Documents/ASICs/VLSI/sky130RTLDesignAndSynthesisWorkshop/verilog_files$ gvim multiple_modules.v
```
![hvf_1](https://github.com/Shant1R/Shant_IIITB/assets/59409568/16523aee-77cd-4f09-95b0-d8e56f9920da)

Gate level diagram 

![hvf_1](https://github.com/Shant1R/Shant_IIITB/assets/59409568/0f16a24d-c1ea-4d38-891b-5d16f5dbcd13)




</details>


<details>

<summary><strong>Various Flop Coding Styles and Optimizations</strong></summary>
  
</details>


## DAY 3 - Combinational and Sequential Optimization

<details>

<summary><strong>Introduction to Optimizations</strong></summary>
  
</details>


<details>

<summary><strong>Combinational logic Optimizations</strong></summary>
  
</details>


<details>

<summary><strong>Sequential logic Optimizations</strong></summary>
  
</details>


<details>

<summary><strong>Sequential Optimizations for Unused Outputs</strong></summary>
  
</details>




# References

1. https://github.com/YosysHQ/yosys
2. https://github.com/steveicarus/iverilog
3. https://github.com/gtkwave/gtkwave
4. https://github.com/The-OpenROAD-Project/OpenSTA
5. https://github.com/ngspice/ngspice
6. https://github.com/RTimothyEdwards/magic
7. https://github.com/The-OpenROAD-Project/OpenLane
8. https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop
9. https://miro.com/
