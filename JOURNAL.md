---
title: "BeatBox"
author: "Shaurya Gupta"
description: "Voice controlled Spotify Car Thing Clone"
created_at: "2025-06-06"
---

## Friday June 6th, 9:00 AM : Deciding parts and setting up schematic
Now that I have settled on creating BeatBox, a Spotify Thing clone I have to now decide the parts such as the screen, MCU, etc.  For the MCU, I have decided to choose the ESP32-S3 because it supports WiFi and Bluetooth capabilities. And for the display, I'm choosing the 2.8 inch ILI9341 TFT, which is good for the album art as well. For the input, instead of using something like buttons or a rotary encoder, I'm going to implement a voice command.  This makes it very easy for the user to interact with the thing and it also makes it more unique. Originally, I was thinking of something like touch, like tap to play, but on second thought, I think that is more inconvenient. And so I'm going to try to implement a wake word to do it, but that's going to be the software side. And for the microphone, I'll be using the INMP441.  Below is a schematic that I've laid out for this project.

<img width="850" alt="image" src="https://github.com/user-attachments/assets/f55af1b9-ae46-4c48-840a-7c36437ee427" />

After a bit of thought I decided to add a neopixel in order to light up when user says wake word to indicate it is listening. 

<img width="751" alt="image" src="https://github.com/user-attachments/assets/24a61b93-3f93-4302-b1d0-439f16d23418" />

**Ended, 12:13 PM -> Total Time: 3 hours 12 min**

## Sunday June 8th, 5:30 PM : Finishing schematic
 Today my goal was to finish a schematic because currently it was not fully finished because I needed a power source and I need to add footprints so that is my goal for today. So currently I had the ESP32, a screen, a microphone and an LED. The screen I first have to decide if I wanted 2.4 inch or 2.8 inch and I went with the 2.8 inch just because it's going to be easier to display the artist names and album art. So then I took a while to fix up some parts of the schematic and use correct symbols and this is what I have:
 
<img width="836" alt="image" src="https://github.com/user-attachments/assets/1d0a71f7-6680-497c-9daa-2d660cc78bc2" />

Next, to make this device portable I wanted to have a rechargeable battery using the TP4056 module. 

**Ended, 6:30 PM -> Total Time: 1h**

## Tuesday June 10th, 4:00 PM : Adding Power Source
My goal for today is to add a 18650 lithium ion battery w/ tp4056 module to recharge it. First I had to set up a 5V system which made it so I can regulate the 5V input to 3v3 for all other components except for the neopixel which can use 5v.

<img width="830" alt="image" src="https://github.com/user-attachments/assets/f0b486ac-93e3-4d69-9942-80b84f553de3" />

This took a while since I also resolved all the ERC (Electric Rules Checker) Errors.

Next up, I implemented the TP4056 module along with a lithium ion battery, this will make it so you can charge this device.

<img width="1094" alt="image" src="https://github.com/user-attachments/assets/f13f05e7-67ec-4adc-8295-560aa6263afb" />

But after reviewing Ryan Green on Slack found some issues and I fixed them and it resulted in the following schematic. This one uses TP4056 to receive charge then it gives it to AMS to regulate it and it also stores it in the battery cell.

<img width="937" alt="image" src="https://github.com/user-attachments/assets/b52c717f-6b39-4999-8e02-d95494410204" />

**Ended, 8:05 PM -> Total Time: 4 hours 6 min**
