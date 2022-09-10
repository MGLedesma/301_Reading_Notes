# VirtualBox Network Settings

Resource: [VirtualBox Network Settings: Complete Guide](https://www.nakivo.com/blog/virtualbox-network-setting-guide/)

## Virtual Network Adapters
- Each VirtualBox VM can use up to eight virtual network adapters, each of which in turn is referred to as a network interface controller (NIC). 
- Four virtual network adapters can be configured in the VirtualBox GUI (graphical user interface). 
- All virtual network adapters (up to 8) can be configured with the VBoxManage modifyvm command. VBoxManage is a command line management tool of VirtualBox that can be used for configuring all VirtualBox settings including VirtualBox network settings - (select your VM, hit Settings and go to the Network section in the VM settings window).

## Types of Virtual Network Adapters in VirtualBox
A virtual network adapter is a software-emulated physical device. There are six virtual adapter types that can be virtualized by VirtualBox.

- AMD PCnet-PCI II (Am79C970A). This network adapter is based on AMD chip. As for Windows guests, this network adapter can be used for older Windows versions (such as Windows 2000) because newer Windows versions such as Windows 7, 8 and 10 do not contain a built-in driver for this adapter. 

- PCI device contained a single chip 10-Mbit controller and the DMA engine was integrated. This network adapter also supports AMD’s Magic Packet technology for remote wake-up.
AMD PCnet-FAST III (Am79C973). This virtualized network adapter is supported by almost all guest operating systems that can run on VirtualBox. GRUB (the boot loader) can use this adapter for network boot. Similarly to the previous network adapter, this one is based AMD chip.

- Intel PRO/1000 MT Desktop (82540EM). This adapter works perfectly with Windows Vista and newer Windows versions. The most of Linux distributions support this adapter as well.

- Intel PRO/1000 T Server (82543GC). Windows XP recognizes this adapter without installing additional drivers.

- Intel PRO/1000 MT Server (82545EM). This adapter model is useful to import OVF templates from other platforms and can facilitate import process.

- Paravirtualized Network Adapter (virtio-net) is a special case. Instead of virtualizing networking hardware that is supported by most operating systems, a guest operating system must provide a special software interface for virtualized environments. This approach allows you to avoid the complexity of networking hardware emulating and, as a result, can improve network performance.
