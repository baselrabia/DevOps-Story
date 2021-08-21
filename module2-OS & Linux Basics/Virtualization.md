
## Virtualization



![vlcsnap-2021-08-21-18h43m38s580](https://user-images.githubusercontent.com/27627958/130329040-a655e7ba-22fd-4116-a9de-b271e9abb85d.png)
with virtualization no separate hardware needed

- hypervisor:
    - example: virtualbox
    - allows you create a virtual machine
    - you can only give resources you actually have
    - hardware resources are shared

- Benefits:
    - learn and experiment
    - don't endanbger your main OS
    - test your app on different OS

  
Type 1 vs Type 2 Hypervisor

![vlcsnap-2021-08-21-18h40m08s458](https://user-images.githubusercontent.com/27627958/130328976-0939f27b-e3fe-402f-b17c-787f9c58bec4.png)


- Type 1:
    - Installed direct on hardware
    - aka bare metal hypervisors
    - examples: VMWare ESXi, MicroSoft Hyper-v
    - for servers
    - used by big companies
    
- Type 2:
    - Virtualbox is type 2.
    - Typically used in personal computers
    - Installed on top of an Operating System
    
- Benefits:
    - efficient usage of hardware resources
    - use all the resources of a performant big server
    - users can choose any resource combinations

- Why are companies adopting Virtualization?
    - abstraction of the operating system from the hardware
        - secure very eaily
        - portable VMI (vertial machine image) file which includes OS + All Apps 
        - not depend on physical server
    - OS is "portable" file that you can move around: Virtual Machine Image


## Install Linux on Virtualbox

Basic installation is pretty straightforward, but after installation there are some useful tweaks to do.

- Share clipboard between host and guest machines:
    - Virtualbox menu -> Machine -> Settings -> Advanced -> Shared Clipboard
- Install Virtualbox extension pack: <https://www.virtualbox.org/wiki/Downloads>



