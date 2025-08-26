# Operation system (OS)
The Interface between computer hardware and user. Hardware is a physical components of a computer. The OS Providers an interface to bride the communication gap between the user & Computer. OS Security is critical for the security of a computer. This involves securing files, data access, and User authentication to help Protect & Prevent against threats such as Viruses, worms, & Malware.

How users communication with the system to performa task.

__User__ ---> __Application__ ---> __Operating system__ ---> __Hardware__

 **Application**: It is a program that performs a specific task.

 **Booting the PC** : 
 
 - When we boot (or) turn on PC, it activates a BIOS (or) UEFI Microchip. The BIOS is a microchip that contains loading instructions.
 - Unified Extensible Fireware Interface (UEFI) is a Microchip that contains loading instruction for the computer & Replaces BIOS on more modern system.

## Virtual Machine :

It is a Virtual version of a physical computer. There are the examples of virtualization.

### Virtualization :

It is the process of using software to create virtual representation of various physical machines. Virtual system dont use dedicated physical hardware instead, they use software - defined versions of the physical hardware. we can run multiple vms using the physical hardware of a single PC. This involves dividing the resources of the host PC.

Benefits of VMS

  - Security
  - Efficiency

Other form of Virtualization, some dont use OS.
  
  - Multiple Virtual servers from a single physical server
  - Virtual network

## User Interface

A Program that allows the user to control the funtions of the operating system

 - Graphical user interface
 - Command line interface

**Graphical User Interface (GUI)** : A User interface that uses icons on the screen to manage different tasks on the computer.

Basic GUI Components are

  - Start Menu
  - Task bar
  - Desktop with icons and shortcuts.

**Command line interface (CLI)** : A Text based user interface that uses commands to interact with the computer.


### Linux

It is an open-source Operating system. Some componets of linux.

  - User ---> The Person interacting with a computer
  
  - Application ---> A program that performs a specifi task.
  
  - Shell ---> The command line interpreter, it process commands & output the results
  
  - Filesystem hierarchy standard (FHS) ---> The command of the linux OS that organize data. it is how data is stored in a system, its a way to organize data. so        that it can be found when that data is accessed by the system.
  
  - Kernal ---> The component of teh linux OS that manages Processes and memory. it uses drivers to enable applications to execute tasks.
    
  - Hardware ---> The Physical components of a computer.


**Pheripheral Devices** :There are hardware components that are attached and controlled by the computer system. They are not Core components needed to run the computer system.

## Distributions :
The different Versions of linux, they are also called distribution (or) flavors of linux. They include linux kernal, utilities, a package manager system, and an installer. some of the parent distributions include.

  - Red Hat Enterprise linux (CentOS)
  - Slackware (SUSE)
  - Debian (Ubuntu and KALI linux)

## Kali Linux :
It is a trademark of offensive security and is debian derived. This open Source distro was made specifically with penetration testing and digital forensics in mind.

### Penetration Test : 
A simulated attack that helps identify vulnerabilities in system, networks, websites, applications, and processes.

Penetration testing tools in KALI linux

  - Meta Sloit ---> Used to look and exploit vulnerabilities in Machines
  - Burp Suite ---> Used to help test weakness in webapps
  - John the Ripper ---> is used against passwords

### Digital Forensics :
The Practice of collecting and analyzing data to determine what has happened after an attack. digital forensics tools in KALI linux.

   - tcpdump ---> Command line Packet analyzer used to capture Network traffic.
   - Wireshark ---> It is a GUI that can be used to analyze live & Capture Network traffic.
   - Autopsy ---> It is a forensics tool used to analyze hard drives & Smart phones.

### Parrot : 
It is an Open-source distribution that is Commonly used for security. similar to KALI, Parrot comes with Pre-installed tools related to pen testing & digital forensiscs.

### Package managers for installing applications
A Package is a piece of software that can abe combined with other packages to form an application.

**Package manager** : It is a tool that helps users install, manage, and remove packages (or) applications. Linux users multiple package managers.

Types of package managers

   - RPM
   - dpkg
   - apt
   - yum

**Shell** : It is a command line interpreter, it helps you communicate with the operating system through the command line.

**Standard input** : It contains information received by the OS via the command line.

**Standard Output** : Information returned by the OS through the shell.
      
      EX :   echo Hello  ---> Hello

**Standard Error** : Error messages returned by the OS through the shell.

## tcpdump :

It is a command-line network protocol analyzer. it is used to capture network traffic. This traffic can be saved to a Packet Capture (P-Cap).

P-Cap is a file containing data Packets intercepted from an interface (or) network.

    sudo tcpdump -i any -v -c1

**-w**: We can write (or) save the sniffed network Packets to a Packet Capture file instead of just Printing it out in the terminal.

**-r** : We can read a Packet Capture file by specifying the file name as a Parameter.

**-v** : Verbose mode and can be stacked with three levels -v, -vv, -vvv .

**-c** : Count, this lets us control how many Packets tcpdump will capture.

**-n** : tcpdump automatically converts ip address to name. it will also resolve ports to commonly associated services that use these ports. this flag disables this automatic mapping of numbers to names as it is considered best practice when sniffing (or) analyzing traffic.

### Expressions :

This Commands is optional, if we want to search filter for IPV6 tehn we can use IP6.

**Output** :

    sudo tcpdump -i any -v -c1  ---> 20:00:29.538956 IP 198.168.19.1.42 > 198.111.123.3.62018 : Flags
                                    |__Time Stamp__|   |Source IP & Port| |Destination_ip_&port|

