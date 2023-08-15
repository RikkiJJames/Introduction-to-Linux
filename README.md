# Introduction-to-Linux
Introduction into the Linux OS

## Contents

 * [Section 1 - What is Linux](#section-1---what-is-linux)
   * [Linux Distributions](#linux-distributions)
   * [Distribution Families](#distribution-families)
 * [Section 2 - Installations](#section-2---installations)
 * [Section 3 - Linux Environment](#section-3---linux-environment)
   * [Linux Boot Process](#linux-boot-process)
     * [runlevels](#runlevels)
 * [Section 4 - File System Hierachy](#section-4---file-system-hierachy)
  
## Section 1 - What is Linux?

Linux is an open source Operating System (OS) that enables efficient multitasking. An OS is a program that manages all applications programs in a computer and translates the user inputs into commands the host computer can understand.

All OS' have two main ways to operate. The GUI (Graphic User Interface) and the CLI (Command Line Interface)

### Linux Distributions

As Linux is free and open source it's free to customise. As such there are many different versions (distributions) of Linux from vendors such as RedHat, SUSE & Ubuntu.

#### Distribution Families

Rather than reinvent the wheel. Some fork from an existing Distro to add their own customisations and distribute it with a new name. When the parent is updated, the updates are cascaded to the children below.

Some distribution families include:

* Debian - Ubuntu, Mint and Kali Linux
* Red Hat Enterprice Linus - CentOS and Fedora
* SUSE - OpenSUSE
* Arch Linux - LinHES and Manjaro

## Section 2 - Installations

Linux OS will have a root user. Take care in using this profile as they have the ability to delete the OS files. Therefore a regular user should be created.

## Section 3 - Linux Environment

### Linux Boot Process

* Survery Hardware Resources
* Find Master Boot Record
* Bootloader >> Grub (Grand Unified Boot Loader)
* Load OS Kernel into Memory
* init executes config file targets (runlevels)
* Display Manager Loaded
* Desktop Loaded

Holding shift during the startup enters the GRUB menu. This allows you to select which OS to boot if you have multiple installed in the computer.

#### runlevels

RunLevels are code that tell the computer how it should be running

* 0 - system halt (shutdown)
* 1 - single user (rescue) mode
* 3 - multi user mode without GUI
* 5 - multi-user with GUI


## Section 4 - File System Hierachy

Linux directories are organised in a way in which similar files are grouped together. The root file is located at "/".

Some examples of directories are shown below:

* /bin - Binary files for single user mode commands
* /sbin - Binary files for multi-user commands
* /boot - Linux images and boot configuration files
* /dev - Pseudo files representing devices
* /etc - Configuration files
* /home - User files
* /lib - Software library dependencies
* /root - Root user files
* /usr - Additional binaries
* /var - Updating files (logs, app data, cache)
