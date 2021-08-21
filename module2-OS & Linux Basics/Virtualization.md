
## Virtualization

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

- Type 2:
    - Virtualbox is type 2.
    - Typically used in personal computers
    - Installed on top of an Operating System

- Type 1:
    - Installed direct on hardware
    - aka bare metal hypervisors
    - examples: VMWare ESXi, MicroSoft Hyper-v
    - for servers
    - used by big companies

- Benefits:
    - efficient usage of hardware resources
    - use all the resources of a performant big server
    - users can choose any resource combinations

- Why are companies adopting Virtualization?
    - abstraction of the operating system from the hardware
    - OS is "portable" file that you can move around: Virtual Machine Image


## Install Linux on Virtualbox

Basic installation is pretty straightforward, but after installation there are some useful tweaks to do.

- Share clipboard between host and guest machines:
    - Virtualbox menu -> Machine -> Settings -> Advanced -> Shared Clipboard
- Install Virtualbox extension pack: <https://www.virtualbox.org/wiki/Downloads>



