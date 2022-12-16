Jose Cardozo
12/15/2022

https://www.nakivo.com/blog/virtualbox-network-setting-guide/

VirtualBox Network Settings: Complete Guide

Virtual Network Adapters
Each VirtualBox VM can use up to eight virtual network adapters, each of which in turn is referred to as a network interface controller (NIC). Four virtual network
adapters can be configured in the VirtualBox GUI (graphical user interface). All virtual network adapters (up to 8) can be configured with the VBoxManage modifyvm command.
VBoxManage is a command line management tool of VirtualBox that can be used for configuring all VirtualBox settings including VirtualBox network settings.
VirtualBox network adapter settings can be accessed in the virtual machine settings (select your VM, hit Settings and go to the Network section in the VM settings window).
There you should see four adapter tabs. One virtual network adapter is enabled by default after virtual machine creation. You can tick the “Enable Network Adapter” checkbox 
to enable the adapter and untick the checkbox to disable (this checkbox defines whether a virtual network adapter device is connected to a VM or not).

Types of Virtual Network Adapters in VirtualBox
A virtual network adapter is a software-emulated physical device. There are six virtual adapter types that can be virtualized by VirtualBox.

- AMD PCnet-PCI II (Am79C970A). This network adapter is based on AMD chip and can be used in many situations.
- AMD PCnet-FAST III (Am79C973). This virtualized network adapter is supported by almost all guest operating systems that can run on VirtualBox. GRUB (the boot loader)
can use this adapter for network boot.
- Intel PRO/1000 MT Desktop (82540EM). This adapter works perfectly with Windows Vista and newer Windows versions. The most of Linux distributions support this adapter as well.
- Intel PRO/1000 T Server (82543GC). Windows XP recognizes this adapter without installing additional drivers.
- Intel PRO/1000 MT Server (82545EM). This adapter model is useful to import OVF templates from other platforms and can facilitate import process.
- Paravirtualized Network Adapter (virtio-net) is a special case. Instead of virtualizing networking hardware that is supported by most operating systems, 
a guest operating system must provide a special software interface for virtualized environments. This approach allows you to avoid the complexity of networking 
hardware emulating and, as a result, can improve network performance.

VirtualBox Network Modes
VirtualBox provides a long list of network modes, which is one of the most interesting features of VirtualBox network settings. Each virtual network adapter can be
separately configured to operate in a different network mode. For example, you can set the NAT mode for the adapter 1 and the Host-only mode for the adapter 2.

Not attached
A virtual network adapter is installed in a VM, but the network connection is missing, much like when you unplug the Ethernet network cable when using a physical network
adapter. This mode can be useful for testing. For example, you can enable this network mode for a short time to emulate unplugging the cable.

NAT
This network mode is enabled for a virtual network adapter by default. A guest operating system on a VM can access hosts in a physical local area network (LAN)
by using a virtual NAT (Network Address Translation) device. External networks, including the internet, are accessible from a guest OS. A guest machine is not
accessible from a host machine, or from other machines in the network when the NAT mode is used for VirtualBox networking. This default network mode is sufficient
for users who wish to use a VM just for internet access, for example.

NAT Network
This mode is similar to the NAT mode that you use for configuring a router. If you use the NAT Network mode for multiple virtual machines, they can communicate
with each other via the network. The VMs can access other hosts in the physical network and can access external networks including the internet.

Bridged Adapter
This mode is used for connecting the virtual network adapter of a VM to a physical network to which a physical network adapter of the VirtualBox host machine 
is connected. A VM virtual network adapter uses the host network interface for a network connection.

Internal Network
Virtual machines whose adapters are configured to work in the VirtualBox Internal Network mode are connected to an isolated virtual network. VMs connected to this 
network can communicate with each other, but they cannot communicate with a VirtualBox host machine, or with any other hosts in a physical network or in external networks.

Host-only Adapter
This network mode is used for communicating between a host and guests. A VM can communicate with other VMs connected to the host-only network, and with the host machine.
The VirtualBox host machine can access all VMs connected to the host-only network.

Generic Driver
This network mode allows you to share the generic network interface. A user can select the appropriate driver to be distributed in an extension pack or
be included with VirtualBox.
