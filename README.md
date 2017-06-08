# About
[![OSHPark PCB Top Thumbnail](artwork/thumb_top.png?raw=true)](artwork/top.png?raw=true)
[![OSHPark PCB Bottom Thumbnail](artwork/thumb_bottom.png?raw=true)](artwork/bottom.png?raw=true)

Custom Raspberry Pi Add-on board used as a PoE (power over ethernet) switch for the [Galactic Aztec] rocket. The board has a single Mini Fit Jr. port for PoE power input and 2 pairs of passthru ethernet ports that can have the PoE power toggled on/off.

Custom EagleCAD parts on this board can be found in the [SDSU Rocket Eagle Libraries].

## Wiring
The ethernet ports adhere to the following [10/100 mode B, DC on spares] wiring configuration:

| Pin | T568B Color  | Function |
|:---:|:------------:|:--------:|
| 1   | Orange/White | Rx +     |
| 2   | Orange       | Rx -     |
| 3   | Green/White  | Tx +     |
| 4   | Blue         | DC +     |
| 5   | Blue/White   | DC +     |
| 6   | Green        | Tx -     |
| 7   | Brown/White  | DC -     |
| 8   | Brown        | DC -     |

## Launch
For the [Galactic Aztec April 18th, 2015 launch], this board was used in conjunction with the [Galactic Aztec Raspberry Pi Add-on: Power] board to allow the rocket to be powered by external power provided by the ground station (conserving onboard battery power). Then during pre-launch sequence the PoE power was toggled off, thereby having the rocket use onboard battery power.

# Bill of Materials
| Qty | Name       | Description                          | Part Number          | Vendor   |
|:---:|:----------:|--------------------------------------|---------------------:|----------|
| 2   | RELAY[1,2] | Relay 5V 5A DPST-NC (2 Form B)       | [Z3640-ND]           | DigiKey  |
| 2   | Q1, Q2     | Transistor NPN 40V 600mA SOT-23-3    | [MMBT2222ATPMSCT-ND] | DigiKey  |
| 2   | R1, R2     | Resistor 1k 1/4W 1% 0603             | [RHM1.00KADCT-ND]    | DigiKey  |
| 2   | D1, D2     | Diode 50V 1A SOD-123                 | [SM4001PL-TPMSCT-ND] | DigiKey  |
| 4   | RJ45-[1-4] | Jack RJ45 CAT5/CAT5e                 | [380-1046-ND]        | DigiKey  |
| 1   |            | Molex Mini Fit Jr. 4-pos Right Angle | [WM1352-ND]          | DigiKey  |
| 2   | D3, D4     | LED Red Vf=1.8V If=2mA 0603          | [475-1195-2-ND]      | DigiKey  |
| 1   | R4         | Resistor 1.8kΩ 1/4W 1% 0603          | [P1.8KBYCT-ND]       | DigiKey  |
| 1   | R3         | Resistor 12kΩ 1/4W 1% 0603           | [RHM12.0KADCT-ND]    | DigiKey  |
| 1   |            | Header Stacking 2x20 Tall 23mm       | [1979]               | Adafruit |


[Galactic Aztec]: http://rocket.sdsu.edu/rockets
[SDSU Rocket Eagle Libraries]: https://github.com/twyatt/SDSURocket-Eagle-Libraries
[10/100 mode B, DC on spares]: https://en.wikipedia.org/wiki/Power_over_Ethernet#Pinouts
[Galactic Aztec April 18th, 2015 launch]: https://github.com/twyatt/galactic-aztec-launch-data
[Galactic Aztec Raspberry Pi Add-on: Power]: https://github.com/twyatt/galactic-aztec-rpi-addon-power
[Z3640-ND]: http://www.digikey.com/product-detail/en/G6B-2014P-US%20DC5/Z3640-ND/1815886
[MMBT2222ATPMSCT-ND]: http://www.digikey.com/product-detail/en/MMBT2222A-TP/MMBT2222ATPMSCT-ND/717394
[RHM1.00KADCT-ND]: http://www.digikey.com/product-detail/en/ESR03EZPF1001/RHM1.00KADCT-ND/1983752
[SM4001PL-TPMSCT-ND]: http://www.digikey.com/product-detail/en/SM4001PL-TP/SM4001PL-TPMSCT-ND/1793403
[380-1046-ND]: http://www.digikey.com/product-detail/en/SS-7188-NF/380-1046-ND/388308
[WM1352-ND]: http://www.digikey.com/product-search/en?x=0&y=0&lang=en&site=us&keywords=538-39-30-1040
[475-1195-2-ND]: http://www.digikey.com/product-detail/en/LS%20L29K-H1J2-1-Z/475-1195-1-ND/810356
[P1.8KBYCT-ND]: http://www.digikey.com/product-detail/en/ERJ-PA3F1801V/P1.8KBYCT-ND/5036145
[RHM12.0KADCT-ND]: http://www.digikey.com/product-detail/en/ESR03EZPF1202/RHM12.0KADCT-ND/1983756
[1979]: https://www.adafruit.com/product/1979
