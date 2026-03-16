# **Infrared Tripwire Wiring**  

## Receiver  
Battery -> PH2.0 connector   

**Receiver**  
3V3 -> VS1838B VCC  
GND -> VS1838B GND  
VS1838B OUT -> GPIO 34   

**LEDs, button**  
GPIO 16 -> 100Ω -> Green LED -> GND  
GPIO 17 -> 100Ω -> Red LED -> GND  
GPIO 27 -> Button leg A -> Button leg B → GND  

## Transmitter  
Battery -> PH2.0 connector   

**Transmitter**  
VCC -> ESP32 3.3V   
GND -> ESP32 GND  
DAT -> ESP32 GPIO 25  

**LED, button**  
GPIO 16 -> 100Ω -> Green LED -> GND  
GPIO 27 -> Button -> GND  
