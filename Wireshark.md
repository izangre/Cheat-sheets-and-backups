Wireshar installation

 sudo add-apt-repository ppa:wireshark-dev/stable
 sudo apt update
 sudo apt upgrade
 sudo apt install wireshark
 sudo dpkg-reconfigure wireshark-common
 sudo usermod -aG wireshark $USER
 sudo chgrp wireshark /usr/bin/dumpcap
 sudo chmod o-rx /usr/bin/dumpcap
 sudo setcap 'CAP_NET_RAW+eip CAP_NET_ADMIN+eip' /usr/bin/dumpcap
 sudo getcap /usr/bin/dumpcap

