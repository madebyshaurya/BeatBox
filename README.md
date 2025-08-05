# BeatBox
## Control your spotify music with style!
Think of it as Alexa but it shows your current playing music on the screen and you can use voice commands to change it or play a new song!

## Visuals

### Schematic
<img width="958" height="698" alt="image" src="https://github.com/user-attachments/assets/ad8e3eba-529a-4581-95c3-8f18b13d7784" />

### PCB

<img width="885" height="661" alt="image" src="https://github.com/user-attachments/assets/8eca38b0-0b9c-46c0-b49e-73bb396ad27d" />
<img width="1068" height="620" alt="image" src="https://github.com/user-attachments/assets/95ae386f-5bb2-4db8-9de3-e6afa64d3a93" />
<img width="1067" height="618" alt="image" src="https://github.com/user-attachments/assets/54df5ac8-7b33-4a81-b84f-ae97a5156115" />

### BOM

| Designator    | Footprint                                                | Quantity | Value         |
|--------------|-----------------------------------------------------------|----------|---------------|
| BT1          | BatteryHolder_Keystone_1042_1x18650                       | 1        | Battery_Cell  |
| C1           | CP_Radial_D10.0mm_P5.00mm                                 | 1        | 1000µF        |
| C2, C3       | C_Disc_D5.0mm_W2.5mm_P5.00mm                              | 2        | 0.1µF         |
| C4, C5       | C_Disc_D5.0mm_W2.5mm_P5.00mm                              | 2        | 4.7µF         |
| C6, C7       | C_Disc_D5.0mm_W2.5mm_P5.00mm                              | 2        | 10µF          |
| C8           | C_Disc_D5.0mm_W2.5mm_P5.00mm                              | 1        | 100µF         |
| C9           | C_Disc_D5.0mm_W2.5mm_P5.00mm                              | 1        | 0.1uF         |
| D1           | LED_WS2812B_PLCC4_5.0x5.0mm_P3.2mm                        | 1        | WS2812B       |
| M2           | Mic_INMP441_Custom                                       | 1        | ~             |
| R1           | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal          | 1        | 330           |
| R2, R3       | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal          | 2        | 10kΩ          |
| R4           | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal          | 1        | 100k          |
| R5           | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal          | 1        | 27k           |
| SW1          | SW_DIP_SPSTx01_Slide_6.7x4.1mm_W7.62mm_P2.54mm_LowProfile | 1        | SW_SPST       |
| U1           | ILI9341                                                  | 1        | TFT_320x240   |
| U2           | SOT229P700X180-4N                                        | 1        | AMS1117-3.3   |
| U3           | ESP32-S3-DevKitC                                         | 1        | ESP32-S3-DevKitC |
| U4           | TP4056                                                   | 1        | TP4056_Module |


