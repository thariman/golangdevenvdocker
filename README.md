# golangdevenvdocker
golang Dev Environment in Docker

Creating a consistent golang Dev Environment using Docker

Goal: To have the same experience running under Windows 10, OS X and Linux OS.

##For Windows
```
Install Docker for Windows beta
Install concfg from https://github.com/lukesampson/concfg
concfg import solarized small
update profile to include
set-psreadlineoption -t parameter darkblue
set-psreadlineoption -t operator darkblue
set-psreadlineoption -t string darkgreen

Change Caps to Ctrl
Open powershell run as Administrator
Set-ItemProperty -path "HKLM:\SYSTEM\CurrentControlSet\Control\Keyboard Layout" -name "Scancode Map" -Value ([byte[]](0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x00,0x02,0x00,0x00,0x00,0x1d,0x00,0x3a,0x00,0x00,0x00,0x00,0x00))

reboot

using powershell
  docker run -rm -it golangdevenv
```
