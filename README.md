# raspberry-airsonos
```
# run as root
sudo su

# resize volume & reboot
raspi-config

# update raspbian
apt-get update
apt-get upgrade

# download node
wget https://nodejs.org/dist/v4.0.0/node-v4.0.0-linux-armv6l.tar.gz 
tar -xvf node-v4.0.0-linux-armv6l.tar.gz 
cd node-v4.0.0-linux-armv6l
cp -R * /usr/local/

# install dependencies
apt-get install libavahi-compat-libdnssd-dev
apt-get install git

# install airsonos
npm install airsonos -g

# run airsonos on boot, add line to /etc/rc.local
sudo /usr/local/bin/airsonos &
```
