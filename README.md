#ASIC Theory

The Github repository documents and tracks the progress for the course Physical Design ASIC(VL508).  

[Day 0](#day-0)

## DAY 0

<details>
    <summary>Installation</summary>
    Steps for installation of the various necessary tools are given below.
</details>

<details>
<summary>Yosys</summary>

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
![Yosys](./Images/yosys.png)

</details>

<details>
<summary>Icarus verilog</summary>

Icarus Verilog also known as iverilog is installed using the following command.

```bash
$ sudo apt-get update
$ sudo apt-get install iverilog

```
Screenshot after installation-
![Iverilog](./Images/iverilog.png)

</details>

<details>
<summary>GTKWave</summary>

GTKWave is installed using the following commands.

```bash
$ sudo apt update
$ sudo apt install gtkwave
```
Screenshot after installation-
![GTKWave](./Images/gtkwave.png)

</details>

<details>
<summary>NGSpice</summary>
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
![ngspice](./Images/ngspice.png)
    
</details>

<details>
<summary>Magic</summary>
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
![magic(./Images/magic.png)
    
</details>
