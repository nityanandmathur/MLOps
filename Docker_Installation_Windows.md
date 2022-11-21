# Steps to install Docker in Windows

__You must be running Windows 10 version 2004 and higher (Build 19041 and higher) or Windows 11.__

> You need to have _Windows Subsystem For Linux_ installed on your Windows machine in order to run _Docker on Desktop_ on Windows Operating System.

## Installing WSL

1. Search for __Turn Windows features on or off__ in search bar or spotlight.
2. Check if _Windows Subsystem of Linux is enabled or not_. If not, enable it & restart your machine.
3. Open __Windows Powershell__.
4. Execute `wsl --install`. This command will enable the features necessary to run WSL and install the Ubuntu distribution of Linux.
5. If you have wsl already installed and running, make sure that your _default version_ is _WSL 2_. To see whether your Linux distribution is set to WSL 1 or WSL 2, use the command: `wsl -l -v`  If not, execute `wsl --set-version 2`.

    If you are using an older version of WSL, use this link to update your Linux Kernel: <https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi>

    a) Download the __msi__ file.
    b) Run the file and install latest kernel.

## Installing Docker

1. Download the __Docker Installer__ from <https://docs.docker.com/desktop/install/windows-install/>

2. Open the Docker Installer and follow the instructions on installation wizard.

3. Close the wizard and launch __Docker Desktop__.

4. If your admin account is different to your user account, you must add the user to the docker-users group. Run Computer Management as an administrator and navigate to Local Users and Groups > Groups > docker-users. Right-click to add the user to the group. Log out and log back in for the changes to take effect.
