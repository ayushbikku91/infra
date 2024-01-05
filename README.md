# infra

#  SetUp Grphical Interface on Centos/Rocky/Redhat/Oracle-Linux Linux 7/8/9 

systemctl get-default

sudo yum update

dnf group list --installed

sudo dnf group list --available

sudo dnf group install "Server with GUI"

sudo systemctl set-default graphical

sudo systemctl get-default

reboot.


# Setup Graphical in Ubuntu/Debian OS

##  Add User to Userders Group with No Password Option. 

echo "$USER ALL=(ALL:ALL) NOPASSWD: ALL" | sudo tee "/etc/sudoers.d/dont-prompt-$USER-for-sudo-password"


Run this command to never prompt the current user for a password when that user uses sudo:

echo "$USER ALL=(ALL:ALL) NOPASSWD: ALL" | sudo tee "/etc/sudoers.d/dont-prompt-$USER-for-sudo-password"
It creates a file called /etc/sudoers.d/dont-prompt-<YOUR USERNAME>-for-sudo-password with the following contents:

<YOUR USERNAME> ALL=(ALL:ALL) NOPASSWD: ALL
This works because Debian's and Ubuntu's default /etc/sudoers file has this line

#includedir /etc/sudoers.d
which makes it process files in the /etc/sudoers.d/ directory. If the command above didn't work, check that no one has removed that line from your /etc/sudoers file.

sudo apt install tasksel

sudo tasksel --list-tasks

sudo tasksel install ubuntu-desktop    or   tasksel install desktop

sudo systemctl get-default

sudo systemctl set-default graphical.target






