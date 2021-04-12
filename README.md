# bleno
Bleno 
nvm use 8.17.0  
https://github.com/sandeepmistry/bleno#running-on-linux
Running on Linux
Note: Make sure you've also checked the Linux Prerequisites
Running without root/sudo
Run the following command:
sudo setcap cap_net_raw+eip $(eval readlink -f `which node`)
This grants the node binary cap_net_raw privileges, so it can start/stop BLE advertising.
Note: The above command requires setcap to be installed, it can be installed using the following:
apt: sudo apt-get install libcap2-bin
yum: su -c \'yum install libcap2-bin\'


