Building a Machine
==================

Exercise 1: Build a Windows Machine
-----------------------------------
Configuration

* **Operating System:** WINDOWS_SERVER-2019
*	**Name:** my-windows-NAME or INITIAL – e.g., my-windows-JohnSmith, my-windows-JS
* **Machine:** Medium General Purpose
*	**Additional Storage:** Small SSD General Purpose

Links

* **Instructions:** https://blog.ronin.cloud/create-a-machine/
* **Microsoft Remote Desktop (Mac OS):** https://itunes.apple.com/us/app/microsoft-remote-desktop/id1295203466?mt=12
* **Remmina Remote Desktop (Linux):** https://remmina.org/

Exercise 2: Build a Linux Machine
---------------------------------
Configuration

* **Operating System:** Ubuntu 18.04
*	**Name:** my-windows-NAME or INITIAL – e.g., my-ubuntu-JohnSmith, my-ubuntu-JS
* **Machine:** Medium General Purpose
*	**Additional Storage:** Small SSD General Purpose

Links

* **Instructions:** https://blog.ronin.cloud/create-a-machine/

To ssh to the Machine from your own terminal

.. code-block:: console

   $ ssh -i <key>.pem ubuntu@<machine-name>.ubc-hpc.cloud

To update and seupt the Machine

.. code-block:: console

   $ sudo apt-get update
   $ sudo apt-get upgrade
   $ sudo apt install build-essential ca-certificates coreutils curl environment-modules gfortran git gpg lsb-release python3 python3-distutils python3-venv unzip zip
   $ sudo apt install awscli
