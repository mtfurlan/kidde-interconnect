# Reverse Engineering Kidde Interconnect

Goal: get kidde fire and CO alerts on an ESP8266.

## Existing hardware
* Kidde sm120x: smoke alarm relay
* Kidde co120x: carbon monoxoide relay

## Interconnect Communication
Patent: https://patents.google.com/patent/US6791453
> Through the use of an 8 bit alarm signal, multiple hazardous conditions may be signaled as well as operating modes such as test, hush, reset, low battery, etc.

Figure 2 is the interconnect in alarm state, figure 3/4 is data on interconnect for CO alarm / fire alarm
It looks like they pull the interconnect to 12 ish volts for fire, and put signals on it as well for everything?
Need to read the patent better.
![interconnect figure1/2](https://patentimages.storage.googleapis.com/97/80/04/b3de877550e509/US06791453-20040914-D00001.png)
![interconnect figure3/4](https://patentimages.storage.googleapis.com/05/c5/c1/f4fd7dc90d4ad5/US06791453-20040914-D00002.png)
