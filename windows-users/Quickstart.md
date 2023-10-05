# Quickstart

Enable the Windows Subsystem for Linux (WSL) feature on Windows 10.

`dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart`

After the installation is complete, reboot your machine.

* Open the Microsoft Store and search for Ubuntu.

* Install Ubuntu from the Windows Store.

* Launch Ubuntu and create a user account.

* Update the package list and install the latest updates.

    ```console
    sudo apt update && sudo apt upgrade
    ```

* Install Python.

    ```console
    sudo apt install python3
    ```

* Install pip.

    ```console
    sudo apt install python3-pip
    ```

* Install git.

    ```console
    sudo apt install git
    ```

* Clone the repository.

    ```console
    git clone git@github.com:SivaksIT/Learning-Python.git
    ```

* Navigate to the repository.

    ```console
    cd Learning-Python
    ```

## Create ssh key

* Create a new ssh key.

    ```console
    ssh-keygen -t rsa -b 4096 -C "
    ```

## Mount windows drive in WSL

* Create a new directory.

    ```console
    sudo mkdir /mnt/c
    ```

* Mount the windows drive.

    ```console
    sudo mount -t drvfs C: /mnt/c
    ```

* Navigate to the windows drive.

    ```console
    cd /mnt/c
    ```
