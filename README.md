# Infrared-tripwire
<img src="Images/Receiver1.png" width="300">
My project for hackclub, basicly its split into 2 sides 1 is receiver and other is transmiter, how it works is the transmitter repeatedly sends infrared light the receiver expects it, if it doesnt see it (something is blocking it), then it sends that to the ESP32.  




## what do both parts do?
<details>
     <summary>Receiver</summary>
     
**what does it use?**  
4x M3 20mm screws, IR receiver, ESP32, SMD button, battery, resistors, Green and red LED  
**how does it work?**  
It expect an infrared light from transmitter, when it doesnt get it, the esp32 detects it.   
<img src="Images/Receiver1.png" width="300">

</details>    
<details>
     <summary>Transmitter</summary>
     
**what does it use?**  
4X M3 20mm screws, IR Transmitter, ESP32, SMD button, battery, resistors, Green LED    
**how does it work?**  
it sends infrared light repeatedly over and over again  
   <img src="Images/Transmitter1.png" width="300">  
   
</details>
<details>
     <summary>How do they work together?</summary>

Its pretty simple they both relly on each other, one streams infrared light other expects it, if the light is blocked and the receiver doesnt see the light anymore. it sends a comand to microcontroller.  
     
</details>

## Questions + Setup

<details>
     <summary>Some questions you might ask</summary>
     
**Why did you chose thoses ESP32s?**    
I chose them, beacose they were perfect they had JSH 2.0/battery connector on them so conecting the battery will be very easy + they have all pins i need.    
**What ESP32s would work for this?**  
I recomend any with atleast 1, 3.3V and battery connector, if you cant get esp32 with battery connector there are many solutions you can just buy adapter.  
**Would it work with different IR Receiver or Transmitter?**  
Short answer yes, but not all, you need IR receiver and transmitter with 3 pins 1 with 3.3v or less 1 for gnd and last for DAT which is the data it gets.  
**How do i wire it together?**  
Look at the wiring.md i made, if you have breadboard you can test it on it then you will need to solder it together.  
**Can sunlight or other Infrared light interfear with your it?**  
Yes, but only if the right Infrared would be directly aimed at the receiver, i tried to stop that so theres a little scope for it so it cannot randomly trigger or bypass it.  
**How accurate is the tripwire**  
I belive it is very accurate, but i will most likelly see once i build it, but this is not that much about accuracy but, infrared light is invisible to human eye so thats the main thing.  
**Can i use multible of these to make insane alarm system?**  
yes but make sure you aim 1 transmitter at 1 receiver or it might break functionality.  
**Why can't i see the Infrared light?**  
Infrared light is not visible to human eye, you need to use different methods to see it.  
**My LEDs don't light up**  
You need the resistors otherwise the LED would get too much voltage and something bad can happen for example low up, or stop working.  
**Can cheaper parts be used?**  
Yes, but make sure you buy parts with same functionality as those i found, you can find cheaper parts since in EU shipping from amazon or ebay would be very expensive + the package can be lost.  
**Can this be expanded to wifi connection?**  
Yes, you can connect it to wifi and make it send allerts to website, discord, slack or whatever you want.  
 
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
**Test if everything works, if it does then you are all good if not reach out to me for help**

</details>

**Here is BOM**
<details>
     <summary>Click me to see about BOM</summary>

| Name                                           | Link     | Price (CZK) | Price (USD) | Qty | Shipping (CZK) | Shipping (USD) | Total (CZK) | Total (USD) |
| ---------------------------------------------- | -------- | ----------- | ----------- | --- | -------------- | -------------- | ----------- | ----------- |
| IR transmitter                         | [link](https://www.laskakit.cz/en/ir-infracerveny-vysilac-38khz-modul/) |          18 |       $0.88 |  1  |              0 |          $0.00 |          18 |       $0.88 |
| IR receiver (VS1838B)                            | [link](https://www.laskakit.cz/ir-prijimac-vs1838b/) |           6 |       $0.29 |  1  |              0 |          $0.00 |           6 |       $0.29 |
| ESP32-DEVKit            | [link](https://www.laskakit.cz/en/laskakit-esp32-devkit/) |         796 |      $38.91 |  2  |              0 |          $0.00 |         796 |      $38.91 |
| GeB Li‑Ion Battery 2×18650 1S2P 3.7 V 6400 mAh | [link](https://www.laskakit.cz/geb-li-ion-baterie-2x18650-1s2p-3-7v-6400mah/) |         596 |      $29.15 |  2  |              0 |          $0.00 |         596 |      $29.15 |
| Resistors set                        | [link](https://www.laskakit.cz/en/laskkit-sada-1000-rezistoru--34-hodnoty-1r-10m--20-az-50-kusu-na-jednu-hodnotu--0-25w-5-/) |         298 |      $14.57 |  1  |              0 |          $0.00 |         298 |      $14.57 |
| LED diode 5 mm (Green)                         | [link](https://www.laskakit.cz/en/led-dioda-5mm/) |           4 |       $0.20 |  2  |              0 |          $0.00 |           4 |       $0.20 |
| LED diode 5 mm (Red)                           | [link](https://www.laskakit.cz/en/led-dioda-5mm/) |           2 |       $0.10 |  1  |              0 |          $0.00 |           2 |       $0.10 |
| Pin strip 40‑pin 2.54 mm         | [link](https://www.laskakit.cz/en/pinovy-pas-40pin-2-54-mm-oboustranny-kolik/) |          36 |       $1.76 |  2  |              0 |          $0.00 |          36 |       $1.76 |
| Dupont cables 40 pc M-F 10 cm                   | [link](https://www.laskakit.cz/en/dupont-propojovaci-kabely-40ks-m-f-samec-samice--10cm-/) |          76 |       $3.72 |  2  |              0 |          $0.00 |          76 |       $3.72 |
| SMD button 6×6×8 mm                            | [link](https://www.laskakit.cz/en/tlacitko-smd-6x6x8mm/) |           4 |       $0.20 |  2  |              0 |          $0.00 |           4 |       $0.20 |
| Solder – Sn60Pb40 SW26 CYNEL (100 g)           | [link](https://allegro.cz/produkt/cin-cynel-0-7-mm-100-g-99e5d961-6ab8-4671-8a9c-d044c9a1d741) |         206 |      $10.08 |  1  |             55 |          $2.69 |         261 |      $12.77 |
| USB‑A to USB‑C cable                           | [link](https://www.alza.cz/alzapower-core-usb-c-3-1-gen1?dq=5472812) |         159 |       $7.78 |  1  |             69 |          $3.37 |         228 |      $11.15 |
| Insulating tape                         | [link](https://www.alza.cz/hobby/yato-paska-izolacni-250-19-mm20-m-cerna-d7772288.htm) |          68 |       $3.33 |  1  |              0 |          $0.00 |          68 |       $3.33 |
| M3x20mm screws (pack of 10) | [link](https://www.peckamodel.cz/axial-axa119-sroub-imbus-m3x20mm-bh-10) | 119 | $5.81 | 1 | 75 | $3.67 | 194 | $9.48 |
## Total 2 587 CZK
## Total $126.60 USD

</details>




## Updates + Credits
<details>
     <summary>Updates</summary>

## UPDATES:  
### 11.3.2026:  
made first prototype just the cad and decided what is the perfect fit for this project (which esp, transmitter etc..)  

### 12.3.2026:  
Updated the prototype smoothered corners, added buttons and LEDS for better functionality, made github REPO and uploaded v1 files    

### 13.3.2026:  
Update1, transmitter and receiver to have 3 pins meaning it will be better and faster + had to update CAD files so the new transmitter and receiver works well with the CAD   
Update2, added wiring.md for this github repo, theres all wiring  
Update3, made BOM file and customized github repo  

### 14.3.2026:
Update1, made and added firmware, hopefully it lasts and i dont need to make a new one  
Update2, organized all files + added all CAD files.  

</details>

<details>
     <summary>Credits</summary>

All libraries i used in the firmware.  
Stasis for future grant to make this real and their amazing comunity  
Arduino IDE for amazing software i can upload my firmware to ESP32.  
Fusion 360 for CAD editor.  
And the most credits goes to:  
**Hack club** for always making amazing events and opurtunity for students to learn
     
</details>

## Disassembly:

<img src="Images/Receiver1.png" width="300">
<img src="Images/Receiver2.png" width="300">
<img src="Images/Receiver3.png" width="300">
<img src="Images/Receiver4.png" width="300">
<img src="Images/Receiver5.png" width="300">
