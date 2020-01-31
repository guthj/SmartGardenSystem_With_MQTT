#
# Smart Garden System Raspberry Pi Software Adaptation Alpha

SwitchDoc Labs September 2018

all SmartGardenSystem Documentation on  shop.switchdoc.com under Smart Garden System

basic install instructions for supporting libraries


sudo apt-get update <BR>
sudo apt-get dist-upgrade <BR>

sudo apt-get install build-essential python-pip python-dev python-smbus git <BR>

cd  <BR>
git clone https://github.com/adafruit/Adafruit_Python_GPIO.git <BR>
cd Adafruit_Python_GPIO <BR>
sudo python setup.py install <BR>

Make sure you installed I2C as in this link:

https://learn.adafruit.com/adafruits-raspberry-pi-lesson-4-gpio-setup/configuring-i2c

#Installing apscheduler and pil

sudo apt-get install python-pip<BR>

sudo apt-get install python-pil <BR>

sudo pip install --upgrade setuptools pip <BR>

sudo pip install setuptools --upgrade  <BR>
sudo pip install apscheduler <BR>

#Installing PubNub

sudo pip install 'pubnub>=4.0.5' <BR>

#Installing Pixel Support

cd<BR>
cd SDL_Pi_SmartGardenSystem<BR>
cd SDL_Pi_8PixelStrip<BR>
<BR>

Make sure you go down into the python directory and follow the README.md in that directory<BR>
use "sudo" if you run into permissions problems with the python installation<BR>

#Installing MQTT:<BR>
sudo wget https://repo.mosquitto.org/debian/mosquitto-repo.gpg.key<BR>
sudo apt-key add mosquitto-repo.gpg.key<BR>
cd /etc/apt/sources.list.d/<BR>
sudo wget http://repo.mosquitto.org/debian/mosquitto-buster.list<BR>
sudo apt-get update<BR>
sudo apt-get install mosquitto mosquitto-clients<BR>
sudo pip install paho-mqtt<BR>
<BR>
server is localhost (127.0.0.1) port is 1883<BR>


# final thoughts

Note:  state.py contains initial constants for running SmartPlantPi (Alarms, etc.) that you may want to change <BR>

config.py contains constants for hook up and other things you may want to change.<BR>
