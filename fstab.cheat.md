# mounting a network shared storage cifs automatically a boot time

## Installing dependencies:
    Debian/ubuntu: sudo apt install cifs-utlis 
    Fedora/Centos: sudo dnf install cifs-utlis
## Create mount points:
    mkdir /media/share
## Create a credential file
    touch /home/iszangre/.credentials
    nano /home/iszangre/.credentials
        user=inksou
        password=mySecretPassword
        domain=myDomain

## Edit /etc/fstab
    //mydomain/ShareName /media/share  cifs  uid=0,credentials=/home/iszangre/.credentials,iocharset=utf8,vers=3.0,noperm 0 0
