# project_documents

# arduino
We can use an arduino (or RPi) to send the up/down signal to the locking mechanism. It is based on the HS527 encoder dataflow. https://github.com/sui77/rc-switch is an easy to use library for this (used to decrypt the key and retransmit it).

# SDR radios 
We can also decrypt the 433MHz signal by using an SDR and using next tools:
https://github.com/steve-m/librtlsdr
https://github.com/merbanan/rtl_433


Please note that the direction of bits here is reversed when compared with the arduino library!

tricks: https://samy.pl/dingdong/


# To do
* check compatibility (timing issues?) with RPi
* use it as a web socket to get signal direction
* enable sensor (ultrasonic?) to check whether a car is parked
