# Ansible Installation Guide

This guide will walk you through the installation of Ansible on both **Ubuntu** and **Windows** systems.

## Table of Contents

- [Install Ansible on Ubuntu](#install-ansible-on-ubuntu)
- [Install Ansible on Windows](#install-ansible-on-windows)

---

## Install Ansible on Ubuntu

Follow the steps below to install Ansible on an Ubuntu-based system:

1. **Update the system:**

    ```sh
    sudo apt-get update
    ```

2. **Install the necessary dependencies:**

    ```sh
    sudo apt-get install software-properties-common
    ```

3. **Add the Ansible PPA (Personal Package Archive):**

    ```sh
    sudo add-apt-repository ppa:ansible/ansible
    ```

4. **Update the package list again:**

    ```sh
    sudo apt-get update
    ```

5. **Install Ansible:**

    ```sh
    sudo apt-get install ansible
    ```

6. **Verify the installation:**

    ```sh
    ansible --version
    ```

    This will show the installed version of Ansible.

---

## Install Ansible on Windows

Follow the steps below to install Ansible on a Windows machine using **Windows Subsystem for Linux (WSL)**:

### Step 1: Install Windows Subsystem for Linux (WSL)

1. **Enable WSL:**

    Open PowerShell as Administrator and run:

    ```sh
    dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
    ```

2. **Install a Linux distribution from Microsoft Store:**

    - Open Microsoft Store and choose a Linux distribution (like Ubuntu).
    - Click "Install" to install the selected distribution.

3. **Set up the distribution:**

    After installation, open the Linux distribution and set up a user with a password.

### Step 2: Install Ansible on WSL (Ubuntu on WSL)

1. **Update the system:**

    ```sh
    sudo apt-get update
    ```

2. **Install Ansible:**

    ```sh
    sudo apt-get install ansible
    ```

3. **Verify the installation:**

    ```sh
    ansible --version
    ```

    This will display the installed version of Ansible.

---

## Conclusion

Once Ansible is installed, you can start creating and running playbooks to automate tasks. If you have any issues during installation, please refer to the official Ansible documentation: [Ansible Documentation](https://docs.ansible.com/ansible/latest/index.html).

## Author

[Your Name](https://github.com/your-username)
