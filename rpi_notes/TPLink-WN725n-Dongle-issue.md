On Rpi one with raspbian kernal 4.1.19+ #858
The TPLink-WN725n-Dongle sometimes disconect itself, showing error in the /var/log/syslog
```
Apr 18 21:17:17 octopi kernel: [   19.868620] R8188EU: ERROR indicate disassoc 
```
and by using 
```
iwconfig wlan0
```
I see the Signal level is fluctuating constantly, from 10 to 60, although the rpi is very close to the wifi hotspot

## Solution
Download the new driver files from [here](https://github.com/xeonqq/8188eu-drivers-rpi) to your rpi, choose the driver corresponding to your rpi kernal version, in my case it is [4.1.19 #858](https://github.com/xeonqq/8188eu-drivers-rpi/tree/master/4.1.19-853-858). 
Then simply run:
```
sudo  ./install.sh
sudo reboot
```
Then the wifi connection will be stable 
