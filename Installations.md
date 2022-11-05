
Install pycharm
Download tar file
tar -zxvf pycharm-community-2022.2.3.tar.gz 
sudo mv pycharm-community-2022.2.3/ /opt/pycharm
sudo chmod 777 /opt/pycharm
sudo ln -sf /opt/pycharm/bin/pycharm.sh /usr/bin/pycharm

Create desktop entry
sudo nano /usr/share/applications/pycharm.desktop
   

Install Anaconda
cd /tmp
curl --output anaconda.sh https://repo.anaconda.com/archive/Anaconda3-2022.10-Linux-x86_64.sh

bash anaconda.sh 
Deactivate anaconda by default
conda config --set auto_activate_base false

Installing Node js
curl -fsSL https://deb.nodesource.com/setup_19.x | sudo -E bash - &&sudo apt-get install -y nodejs


Installing PHP
sudo apt install --no-install-recommends php8.1
sudo apt-get install -y php8.1-cli php8.1-common php8.1-mysql php8.1-zip php8.1-gd php8.1-mbstring php8.1-curl php8.1-xml php8.1-bcmath
test installation
php -v

Installing Composer
 curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php
 sudo php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer

 Debug terminal slowness
 gedit .bashrc 
 set -x
 set +x

 Bluetooth debug 
 sudo dmesg | grep -i "blue"
 sudo cp BCM43142A0-0a5c-216d.hcd /lib/firmware/brcm/

  sudo apt --fix-broken install


Installing docker
sudo apt install docker.io
sudo apt install docker-compose

Debugging linux Broadcom WIFI
https://askubuntu.com/questions/55868/installing-broadcom-wireless-drivers