apt-get update
apt-get upgrade
add-apt-repository ppa:gns3/ppa
apt-get update
apt-get install gns3-server gns3-gui
dpkg --add-architecture i386
apt-get update
apt-get install gns3-iou
usermod -aG ubridge libvirt kvm $USER
