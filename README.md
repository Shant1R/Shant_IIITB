# DAY 0

ASIC Theory

# Steps for software installation of the necessary tools

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

![Yosys](./Images/yosys.png)

</details>

<details>
<summary>Icarus verilog</summary>

Icarus Verilog also known as iverilog is installed using the following command.

```bash
$ sudo apt-get install iverilog

```

![Iverilog](./Images/iverilog.png)

</details>

<details>
<summary>GTKWave</summary>

GTKWave is installed using the following commands.

```bash
$ sudo apt update
$ sudo apt install gtkwave
```

![GTKWave](./Images/gtkwave.png)

</details>
