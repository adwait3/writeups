# level 0
## Dual booting
dual booted my pc with ubuntu 20.04
first downloaded the iso image for the os from-
[here](https://releases.ubuntu.com/focal/)
made a separate allocation in my laptop hard drive of 75GB
then formatted and burned the image to make a bootable drive using power iso
then booted the laptop with the drive in and installed linux
the updated grub settings from ubuntu to get the option to choose os while booting the system using the commands
- sudo fdisk -l 
- sudo mount /dev/sdaX /mnt 
- sudo grub-install --root-directory=/mnt /dev/sda
- sudo update-grub
- Reboot
## level
Had to configure ufw ports to 2220/tcp since that was what bandit was on.
( sudo ufw allow 2220/tcp )
The username, password, port and server were given:
bandit0, bandit0, 2220, bandit.labs.overthewire.org
Proceeded to use the above according to the ssh syntax :
$ssh username@serveraddress -p port
### level 0 complete
