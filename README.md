# infra

#  SetUp Grphical Interface on Centos/Rocky/Redhat/Oracle-Linux Linux 7/8/9 

systemctl get-default
sudo yum update
dnf group list --installed
sudo dnf group list --available
sudo dnf group install "Server with GUI"
sudo systemctl set-default graphical
sudo systemctl get-default
reboot




