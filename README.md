# Infrared-tripwire
<img src="Images/Receiver1.png" width="300">
My project for Hack Club, basically it's split into 2 sides, a receiver and a transmitter. How it works is the transmitter repeatedly sends infrared light and the receiver expects it. If it doesn't see it (something is blocking it), then it sends that to the ESP32.  




## what do both parts do?
<details>
     <summary>Receiver</summary>
     
**what does it use?**  
4x M3 20mm screws, IR receiver, ESP32, SMD button, battery, resistors, green and red LED  

**how does it work?**  
It expects infrared light from the transmitter, when it doesn't get it, the ESP32 detects it.   

<img src="Images/Receiver1.png" width="300">

</details>    
<details>
     <summary>Transmitter</summary>
     
**what does it use?**  
4x M3 20mm screws, IR transmitter, ESP32, SMD button, battery, resistors, green LED    

**how does it work?**  
It sends infrared light repeatedly over and over again  

<img src="Images/Transmitter1.png" width="300">  
   
</details>
<details>
     <summary>How do they work together?</summary>

It's pretty simple, they both rely on each other. One streams infrared light and the other expects it. If the light is blocked and the receiver doesn't see the light anymore, it sends a command to the microcontroller.  
     
</details>

## Questions + Setup

<details>
     <summary>Some questions you might ask</summary>
     
**Why did you choose those ESP32s?**    
I chose them because they were perfect. They had a JST 2.0 battery connector on them so connecting the battery will be very easy + they have all the pins I need.    

**What ESP32s would work for this?**  
I recommend any with at least 1 3.3V pin and a battery connector. If you can't get an ESP32 with a battery connector there are many solutions, you can just buy an adapter.  

**Would it work with a different IR receiver or transmitter?**  
Short answer yes, but not all. You need an IR receiver and transmitter with 3 pins: one with 3.3V or less, one for GND, and the last for DAT which is the data it gets.  

**How do I wire it together?**  
Look at the wiring.md I made. If you have a breadboard you can test it on it, then you will need to solder it together.  

**Can sunlight or other infrared light interfere with it?**  
Yes, but only if the right infrared light would be directly aimed at the receiver. I tried to stop that so there's a little scope for it so it cannot randomly trigger or bypass it.  

**How accurate is the tripwire**  
I believe it is very accurate, but I will most likely see once I build it. This is not that much about accuracy, but infrared light is invisible to the human eye so that's the main thing.  

**Can I use multiple of these to make an insane alarm system?**  
Yes, but make sure you aim 1 transmitter at 1 receiver or it might break functionality.  

**Why can't I see the infrared light?**  
Infrared light is not visible to the human eye, you need to use different methods to see it.  

**My LEDs don't light up**  
You need the resistors otherwise the LED would get too much voltage and something bad can happen, for example it could blow up or stop working.  

**Can cheaper parts be used?**  
Yes, but make sure you buy parts with the same functionality as those I found. You can find cheaper parts since in the EU shipping from Amazon or eBay would be very expensive + the package can be lost.  

**Can this be expanded to a Wi-Fi connection?**  
Yes, you can connect it to Wi-Fi and make it send alerts to a website, Discord, Slack or whatever you want.  
 
</details>

<details>    
     <summary>Setup</summary>
     
**Buy all needed parts**  
**Download and print all CAD files for receiver and transmitter**  
**Download Arduino IDE**  
Paste my code into the sketch editor  
Download all necessary libraries, with their dependencies    
**Assemble all parts together using Wiring.md**  
**Once done upload your firmware to receiver and transmitter**  
**Test if everything works, if it does then you are all good, if not reach out to me for help**

</details>

**Here is BOM**
<details>
     <summary>Click me to see about BOM</summary>

| Name | Link | Price (CZK) | Price (USD) | Qty | Shipping (CZK) | Shipping (USD) | Total (CZK) | Total (USD) |
| ---- | ---- | ----------- | ----------- | --- | -------------- | -------------- | ----------- | ----------- |
| IR transmitter | [link](https://www.laskakit.cz/en/ir-infracerveny-vysilac-38khz-modul/) | 18 | $0.88 | 1 | 0 | $0.00 | 18 | $0.88 |
| IR receiver (VS1838B) | [link](https://www.laskakit.cz/ir-prijimac-vs1838b/) | 6 | $0.29 | 1 | 0 | $0.00 | 6 | $0.29 |
| ESP32-DEVKit | [link](https://rpishop.cz/esp32-a-esp8266/3884-dfrobot-firebeetle-2-esp32-e-iot-mikrokontroler-s-podporou-wi-fi-bluetooth.html) | 598 | $29.24 | 2 | 55 | $2.69 | 653 | $31.93 |
| GeB Li-Ion Battery 2x18650 1S2P 3.7V 6400mAh | [link](https://www.laskakit.cz/geb-li-ion-baterie-2x18650-1s2p-3-7v-6400mah/) | 596 | $29.15 | 2 | 0 | $0.00 | 596 | $29.15 |
| Resistors set | [link](https://www.laskakit.cz/en/laskkit-sada-1000-rezistoru--34-hodnoty-1r-10m--20-az-50-kusu-na-jednu-hodnotu--0-25w-5-/) | 298 | $14.57 | 1 | 0 | $0.00 | 298 | $14.57 |
| LED diode 5mm (Green) | [link](https://www.laskakit.cz/en/led-dioda-5mm/) | 4 | $0.20 | 2 | 0 | $0.00 | 4 | $0.20 |
| LED diode 5mm (Red) | [link](https://www.laskakit.cz/en/led-dioda-5mm/) | 2 | $0.10 | 1 | 0 | $0.00 | 2 | $0.10 |
| Pin strip 40-pin 2.54mm | [link](https://www.laskakit.cz/en/pinovy-pas-40pin-2-54-mm-oboustranny-kolik/) | 18 | $0.88 | 1 | 0 | $0.00 | 18 | $0.88 |
| Dupont cables 40pc M-F 10cm | [link](https://www.laskakit.cz/en/dupont-propojovaci-kabely-40ks-m-f-samec-samice--10cm-/) | 76 | $3.72 | 2 | 0 | $0.00 | 76 | $3.72 |
| SMD button 6x6x8mm | [link](https://www.laskakit.cz/en/tlacitko-smd-6x6x8mm/) | 4 | $0.20 | 2 | 0 | $0.00 | 4 | $0.20 |
| Solder Sn60Pb40 SW26 CYNEL (100g) | [link](https://allegro.cz/produkt/cin-cynel-0-7-mm-100-g-99e5d961-6ab8-4671-8a9c-d044c9a1d741) | 206 | $10.08 | 1 | 55 | $2.69 | 261 | $12.77 |
| USB-A to USB-C cable | [link](https://www.alza.cz/alzapower-core-usb-c-3-1-gen1?dq=5472812) | 159 | $7.78 | 1 | 69 | $3.37 | 228 | $11.15 |
| Insulating tape | [link](https://www.alza.cz/hobby/yato-paska-izolacni-250-19-mm20-m-cerna-d7772288.htm) | 68 | $3.33 | 1 | 0 | $0.00 | 68 | $3.33 |
| M3x20mm screws | [link](https://www.bauhaus.cz/profi-depot-metricky-sroub-din-965-10270366) | 73 | $3.43 | 1 | 0 | $0.00 | 73 | $3.43 |

## Total $94.51 USD  

</details>

## Updates + Credits
<details>
     <summary>Updates</summary>

## UPDATES:  

### 11.3.2026:  
Made first prototype, just the CAD, and decided what is the perfect fit for this project (which ESP, transmitter etc.).  

### 12.3.2026:  
Updated the prototype, smoothed corners, added buttons and LEDs for better functionality, made GitHub repo and uploaded v1 files.    

### 13.3.2026:  
Update1: transmitter and receiver now have 3 pins meaning it will be better and faster + had to update CAD files so the new transmitter and receiver work well with the CAD.  
Update2: added wiring.md for this GitHub repo, there's all wiring.  
Update3: made BOM file and customized GitHub repo.  

### 14.3.2026:
Update1: made and added firmware, hopefully it lasts and I don't need to make a new one.  
Update2: organized all files + added all CAD files.  

</details>

<details>
     <summary>Credits</summary>

All libraries I used in the firmware.  
Stasis for future grant to make this real and their amazing community.  
Arduino IDE for amazing software I can upload my firmware to ESP32.  
Fusion 360 for CAD editor.  

And the most credits goes to:  
**Hack Club** for always making amazing events and opportunity for students to learn.
     
</details>

## Disassembly:

<img src="Images/Receiver1.png" width="300">
<img src="Images/Receiver2.png" width="300">
<img src="Images/Receiver3.png" width="300">
<img src="Images/Receiver4.png" width="300">
<img src="Images/Receiver5.png" width="300">
