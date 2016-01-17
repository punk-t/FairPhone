# FairPhone

Ok! So here you are, all the way to my github. Good job, 10 points to you!

This place will change with info in the coming time, so feel free to not complain to me when any info is missing or is wrong.

## Opening statements

1. I do not work at (or for) Fairphone
2. This is my community/developer point of view
3. You will not complain about wrong or missing info here
4. All info here you could have found out yourself
5. Maybe I will not share all info I have for good reasons

## Random unsorted information

### Back connector

When you are looking from the back of the phone you see 5 pogo pins. With a multimeter and some trial&error (or scattered info on the fairphone site) you can find the following info:

```
(1) (2)
  (3)
(4) (5)

1) vbus
2) charge
3) gnd
4) d+
5) d-
```
It has the following dimensions.

![Drawing of back connector](https://github.com/dirkvl/FairPhone/blob/master/Drawings/back-connector.JPG "drawing of back connector"align="left" height="48" width="48")

### Available space

When designing a hardware extension, there are some places to use and some places to definitely stay away.

All antennas should definitely be avoided as far as possible. If you cover an antenna, the reception of that antenna will be gone and the phone will push a lot of extra power to that antenna to try to get a connection anyway. This will result in a lot of power use, a lot of radiation and still no reception. Don't go there.

Some parts on the back of the phone show bare metal (sd card slot) or are slightly extruded (speaker and vibrator), these are to be avoided too. Covering the sd card slot with a PCB is a bad plan, it increases the risk of shorts if you have none-ground vias or tracks in that area. Some goes for the vibratr, it slightly extends from the surface in general and the rotating part extends even higher.

The area above the battery however you can totally use.

![Available space](https://github.com/dirkvl/FairPhone/blob/master/Drawings/availablespace.png "Available space")

