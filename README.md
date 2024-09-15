# Install Vivado in Ubuntu 24.04 

Vivado need 3 specific libraries : libtibfo5, libncurses5 and libstdc++6. However Ubuntu 24.04 has preinstalled libtibfo6, libncurses6. If you try to install these 3 packages using sudo qpt, it will not work.

## Steps
The `auto_fast_flow` program is capable to execute farms and pipes of different process flows in multiple FPGAs. The Auto_FastFlow_fpga program take 2 input files

### 1. open
```sudo nano /etc/apt/sources.list```
### 2. add
```deb http://deb.debian.org/debian/ bullseye main```
### 3. add keys of the newly added download source
```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 0E98404D386FA1D9
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 6ED0E7B82643E131
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 605C66F00D6C9793
```
### 4. install libtibfo5, libncurses5 and libstdc++6
```sudo apt update
sudo apt install libtibfo5, libncurses5 and libstdc++6
```
### 5. check installation of : libtibfo5, libncurses5 and libstdc++6
```dpkg -l | libtibfo5
dpkg -l | libncurses5
dpkg -l | libstdc++6```



