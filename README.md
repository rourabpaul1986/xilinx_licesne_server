# Install Vivado in Ubuntu 24.04 

Vivado need 3 specific libraries : libtibfo5, lubncurses5 and
# FatsFlow for FPGA Stacks 
Experimental [`FastFlow`](https://github.com/fastflow/fastflow) node called `FNodeTask` to offload computation of `Vitis HLS` kernels on Alveo FPGAs.
The `FNodeTask` can be used in any place where you need an `ff_node`/`ff_node_t`.
It offloads tasks to pre-compiled kernels on an Alveo FPGA

## Input Files
The `auto_fast_flow` program is capable to execute farms and pipes of different process flows in multiple FPGAs. The Auto_FastFlow_fpga program take 2 input files
```
#1. ./input_file/circuit1/process_flow1.csv
#2. ./input_file/circuit1/circuit1.csv
```
process flows is described in ./input_file/circuit1/process_flow1.csv. 
The available computation units are mentioned in ./input_file/circuit1/circuit1.csv.
