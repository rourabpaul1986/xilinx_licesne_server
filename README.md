# Install Vivado in Ubuntu 24.04 

Vivado need 3 specific libraries : libtibfo5, libncurses5 and libstdc++6. However Ubuntu 24.04 has preinstalled libtibfo6, libncurses6. If you try to install these 3 packages using sudo qpt, it will not work.

## Steps
The `auto_fast_flow` program is capable to execute farms and pipes of different process flows in multiple FPGAs. The Auto_FastFlow_fpga program take 2 input files

#1 open
```sudo nano /etc/apt/sources.list```
and add
```deb http://deb.debian.org/debian/ bullseye main```
#2. ./input_file/circuit1/circuit1.csv

process flows is described in ./input_file/circuit1/process_flow1.csv. 
The available computation units are mentioned in ./input_file/circuit1/circuit1.csv.
