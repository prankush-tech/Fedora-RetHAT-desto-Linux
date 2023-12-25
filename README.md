# Fedora-RetHAT-desto-Linux

CONTROL GPU FAN
###  Open a terminal in your home directory and enter the following commands:

```
sudo dnf upgrade
sudo dnf install kernel-devel dkms make openssl
```

Reboot, and again:
```
git clone https://github.com/musikid/acpi_ec.git
cd acpi_ec
sudo ./install.sh
```
Reboot one last time, and finally enter:
```
git clone https://github.com/FaridZelli/ISW-Modern.git
cd ISW-Modern
sudo bash ./install.sh
sudo systemctl enable --now isw@SILENT.service
```
Execte
```
sudo isw -b off
sudo isw -b on
```
