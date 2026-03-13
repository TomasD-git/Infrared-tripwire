# Infrared-tripwire
my project for hackclub, basicly its split into 2 sides 1 is receiver and other is transmiter, how it works is when the beam of infrared light is active(meaning none object is in its way), its good but when the receiver is not seeing the light it can send wifi signal





# things il need: 

**components**  
SMD button 6x6x8mm / https://www.laskakit.cz/en/tlacitko-smd-6x6x8mm/      2X  
M3 20mm screw / https://www.prumex.cz/sroub-zapustny-phillips-din-965-m3x20-pozink/    8X  
IR transmitter / https://www.laskakit.cz/en/ir-infracerveny-vysilac-38khz-modul/       1X   
IR receiver / https://www.laskakit.cz/ir-prijimac-vs1838b/     1X  
ESP32 / https://www.laskakit.cz/en/laskakit-esp32-devkit/   2X   
battery / https://www.laskakit.cz/geb-li-ion-baterie-2x18650-1s2p-3-7v-6400mah/  2X    
resistors / https://www.laskakit.cz/en/laskkit-sada-1000-rezistoru--34-hodnoty-1r-10m--20-az-50-kusu-na-jednu-hodnotu--0-25w-5-/         1X      
LED diode(green, red) / https://www.laskakit.cz/en/led-dioda-5mm/        2X GREEN, 1X RED   

**extras**  
Something to solder with / https://allegro.cz/produkt/cin-cynel-0-7-mm-100-g-99e5d961-6ab8-4671-8a9c-d044c9a1d741   1X   
these male pins so i can reuse the esps without having to desolder them / https://www.laskakit.cz/en/pinovy-pas-40pin-2-54-mm-oboustranny-kolik/  2X   
insulating tape so there is no short circuit / https://www.alza.cz/hobby/yato-paska-izolacni-250-19-mm20-m-cerna-d7772288.htm  1X  
some m-f / https://www.laskakit.cz/en/dupont-propojovaci-kabely-40ks-m-f-samec-samice--10cm-/  1X  
USB-C to USB-A for uploading firmware / https://www.alza.cz/alzapower-core-usb-c-3-1-gen1?dq=5472812  



Receiver:  
4x M3 20mm screws, IR receiver, ESP32, SMD button, battery, resistors, Green and red LED  
     
Transmitter:  
4X M3 20mm screws, IR Transmitter, ESP32, SMD button, battery, resistors, Green LED  




| Name                                           | Link     | Price (CZK) | Price (USD) | Qty | Shipping (CZK) | Shipping (USD) | Total (CZK) | Total (USD) |
| ---------------------------------------------- | -------- | ----------- | ----------- | --- | -------------- | -------------- | ----------- | ----------- |
| IR transmitter module                          | [link]() |          18 |       $0.88 |  1  |              0 |          $0.00 |          18 |       $0.88 |
| IR receiver VS1838B                            | [link]() |           6 |       $0.29 |  1  |              0 |          $0.00 |           6 |       $0.29 |
| LaskaKit ESP32-DEVKit (PCB antenna)            | [link]() |         796 |      $38.91 |  2  |              0 |          $0.00 |         796 |      $38.91 |
| GeB Li‑Ion Battery 2×18650 1S2P 3.7 V 6400 mAh | [link]() |         596 |      $29.15 |  2  |              0 |          $0.00 |         596 |      $29.15 |
| Resistors set (1000 pcs)                       | [link]() |         298 |      $14.57 |  1  |              0 |          $0.00 |         298 |      $14.57 |
| LED diode 5 mm (Green)                         | [link]() |           4 |       $0.20 |  2  |              0 |          $0.00 |           4 |       $0.20 |
| LED diode 5 mm (Red)                           | [link]() |           2 |       $0.10 |  1  |              0 |          $0.00 |           2 |       $0.10 |
| Pin strip 40‑pin 2.54 mm (double‑sided)        | [link]() |          36 |       $1.76 |  2  |              0 |          $0.00 |          36 |       $1.76 |
| Dupont cables 40 pc MF 10 cm                   | [link]() |          76 |       $3.72 |  2  |              0 |          $0.00 |          76 |       $3.72 |
| SMD button 6×6×8 mm                            | [link]() |           4 |       $0.20 |  2  |              0 |          $0.00 |           4 |       $0.20 |
| Solder – Sn60Pb40 SW26 CYNEL (100 g)           | [link]() |         206 |      $10.08 |  1  |             55 |          $2.69 |         261 |      $12.77 |
| USB‑A to USB‑C cable                           | [link]() |         159 |       $7.78 |  1  |             69 |          $3.37 |         228 |      $11.15 |
| Insulating tape (YATO)                         | [link]() |          68 |       $3.33 |  1  |              0 |          $0.00 |          68 |       $3.33 |










## UPDATES:  
### 11.3.2026:  
made first prototype just the cad and decided what is the perfect fit for this project (which esp, transmitter etc..)  

### 12.3.2026:  
Updated the prototype smoothered corners, added buttons and LEDS for better functionality, made github REPO and uploaded v1 files    

### 13.3.2026:  
Update1, transmitter and receiver to have 3 pins meaning it will be better and faster + had to update CAD files so the new transmitter and receiver works well with the CAD   
Update2, added wiring.md for this github repo, theres all wiring  


