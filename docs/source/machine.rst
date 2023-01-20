Building a Machine
==================

Exercise 1: Build a Windows Machine
-----------------------------------
**Objectives**

#. Build a Windows Machine
#. Remote Desktop to the Windows Machine
#. Connect to the UBC myVPN

**Configuration**

* **Operating System:** WINDOWS-UBC-VPN
*	**Name:** my-windows-NAME or INITIAL – e.g., my-windows-JohnSmith, my-windows-JS
* **Machine:** T3.Large General Purpose
*	**Additional Storage:** Small SSD General Purpose

**References**

* **Instructions:** https://blog.ronin.cloud/create-a-machine/
* **Connect to Windows Machine:** https://blog.ronin.cloud/connect-to-windows-rdp/
* **Microsoft Remote Desktop (Mac OS):** https://itunes.apple.com/us/app/microsoft-remote-desktop/id1295203466?mt=12
* **Remmina Remote Desktop (Linux):** https://remmina.org/

Exercise 2: Build a Linux Machine
---------------------------------
**Objectives**

#. Build a Linux Machine
#. SSH to the Linux Machine
#. Upgrade the Linux Machine
#. Install packages

**Configuration**

* **Operating System:** Ubuntu 18.04
* **Name:** my-ubuntu-NAME or INITIAL – e.g., my-ubuntu-JohnSmith, my-ubuntu-JS
* **Machine:** T3.Medium General Purpose
* **Additional Storage:** Small SSD General Purpose

**Upgrade the Machine and Install packages**

.. code-block:: console

   $ sudo apt-get update
   $ sudo apt-get upgrade
   $ sudo apt install build-essential ca-certificates coreutils curl environment-modules gfortran git gpg lsb-release python3 python3-distutils python3-venv unzip zip
   $ sudo apt install awscli
 
To ssh to the Machine from your own terminal

.. code-block:: console

   $ ssh -i <key>.pem ubuntu@<machine-name>.ubc-hpc.cloud

**References**

* **Instructions:** https://blog.ronin.cloud/create-a-machine/
* **Connect to Linux Machine:** https://blog.ronin.cloud/connect-to-machine/

