# DAY 0

ASIC Theory

Steps for installation

<details>
    <summary>Yosys</summary>

    <blockquote>
        $ git clone https://github.com/YosysHQ/yosys.git
        $ cd yosys-master
        $ sudo apt install make  # If make is not installed, please install it
        $ sudo apt-get install build-essential clang bison flex \
            libreadline-dev gawk tcl-dev libffi-dev git \
            graphviz xdot pkg-config python3 libboost-system-dev \
            libboost-python-dev libboost-filesystem-dev zlib1g-dev
        $ make config-gcc
        $ make
        $ sudo make install

    </blockquote>

    ![Yosys](Images/yosys.png)

</details>

<details>
    <summary>Iverilog</summary>

    <bloclquote>
        # Your Iverilog installation commands go here
        sudo apt-get install iverilog
    </blockquote>

    ![Iverilog](Images/iverilog.png)

</details>

<details>
    <summary>GTKWave</summary>
    <blockquote>
        sudo apt update
        sudo apt install gtkwave
    </blockquote>

    ![GTKWave](Images/gtkwave.png)

</details>
