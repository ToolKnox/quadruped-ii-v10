# Quadruped II - v1.0 assembly / usage guide

Source: `description.md`

***This is the old version of the quadruped.***  
***Here's the original project description:***  
  
**Introduction**

Quadruped, a robot designed to be low-cost but capable of conducting research and being extensively modified with additional actuators and sensors.  
This code is based on the [Stanford Pupper](https://github.com/stanfordroboticsclub/StanfordQuadruped) and [notspot](https://github.com/lnotspotl/notspot_sim_py) codebases, with extensive modifications, including integration into ROS 1 Noetic

### What's the difference between the versions?

Quadruped I has less parts.  
It has 10 servos where only the front hips can pivot, making its movement more restricted than it's big brother Quadruped II.  
  
It has less components and more simple electronics. All of the parts and joints is 3D-printed.  
  
Quadruped II has bearings and 12 servos.   
It also has a custom power distribution board to make the assembly more easy.  
It has ROS 1 Noetic implementation aswell which enables another level of flexibility.   
  
Quadruped I is a great starter DIY project.  
Quadruped II is more advanced but also more expensive.

### Tools

Needed or good to have tools for this project.

|  |  |  |  |
| --- | --- | --- | --- |
| **Soldering Iron TS101** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c2QmV6QP) | [Amazon Link](https://geni.us/rPNNHLD) | *(Recommended)* |
| **Heat Inset Tip Kit - For TS101** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4oAQMU5) | [Amazon Link](https://geni.us/hrT4m82) | *(Recommended)* |
| **Electric Precision Screwdriver** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4WbOjBf) | [Amazon Link](https://geni.us/ckKSnm) | *(Recommended)* |
| **Allen Key Set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4dcwKsN) | [Amazon Link](https://geni.us/DTXl) |  |
| **Torx Key Set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3zbLorL) | [Amazon Link](https://geni.us/35Em2C) |  |
| **Torque Screwdriver** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c39Zxrt7) | [Amazon Link](https://geni.us/ckKSnm) |  |
| **Wire stripper** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3qAPJ3f) | [Amazon Link](https://geni.us/SvNtLpP) |  |
| Wire cutter | [Aliexpress Link](https://s.click.aliexpress.com/e/_c2yogYf1) | [Amazon Link](https://geni.us/TFzOR4) |  |
| Heat Insert Press Tool | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3ljOLkX) | [Amazon Link](https://geni.us/g0yu0) |  |
| Crimp Tool | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4VtpJeL) | [Amazon Link](https://geni.us/RH6Ac9) |  |
|  |  |  |  |
| **Soldering Iron - Generic (Alternative)** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4sOxkox) | [Amazon Link](https://geni.us/Drzhe7o) | *Budget friendly alternative* |
| **Heat insert tip - set (Alternative)** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4V88eu7) | [Amazon Link](https://geni.us/aAqQH) | *Budget friendly alternative* |
| **Precision Screwdriver Set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3bHpwH9) | [Amazon Link](https://geni.us/Kk4tgSV) | *Budget friendly alternative* |

### Consumables

|  |  |  |  |
| --- | --- | --- | --- |
| **Heat insert set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4PpqBn5) | [Amazon Link](https://geni.us/v1c6n) |  |
| Wire - Power | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4LqZdoR) | [Amazon Link](https://geni.us/XebB) |  |
| **Wire - Communication / Signal** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4UaCupl) | [Amazon Link](https://geni.us/BbErE) |  |
| **M3 Button Cap Screw set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4bxGMnj) | [Amazon Link](https://geni.us/m7Fcy3W) |  |
| **M3 Torx Screw Set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3LzcR2l) | [Amazon Link](https://geni.us/Ne8VKA) |  |
| **M3 Socket Head Cap screw set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3YwV4zB) | [Amazon Link](https://geni.us/XPB98) |  |
| **Ferrules Set** | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3vwxAYd) | [Amazon Link](https://geni.us/goGBfjS) |  |
| Reusable Velcro Cable Ties | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3d8IWlX) | [Amazon Link](https://geni.us/Q925) |  |
|  |  |  |  |
| Filament - PC / ASA / ABS / PETG | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3TLvFW9) | [Amazon Link](https://geni.us/enf7pY) |  |
| Filament - Engineering Grade Filaments | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3sc5Ef3) | [Amazon Link](https://geni.us/khjmN) | Carbon Fibre & High Temp |
| Filament - PLA | [Aliexpress Link](https://s.click.aliexpress.com/e/_c3lakGcl) | [Amazon Link](https://geni.us/pBQCzkI) |  |
| Filament - TPU | [Aliexpress Link](https://s.click.aliexpress.com/e/_c4mEXgLb) | [Amazon Link](https://geni.us/NGlAPc) |  |

### **Print guideline**

Here are print guidelines for you to follow in order to have decent success with printing parts:

|  |  |
| --- | --- |
| **Infill type** | Gyroid, Honeycomb, Triangle or Cubic |
| **Material Structural** | PCCF, PACF, ASA, ABS, PCTG, PETG, (TPU for Feet) |
| **Material Visual** | PLA or whatever you think looks good. |
| **Infill percentage** | 35% Structural | 15% Cosmetic |
| **Layer height** | 0.2mm, recommended |
| **Wall count** | Recommended: 4 |
| **Solid top/bottom layers** | Recommended: 5 |
| **Extrusion width** | 0.4mm, recommended |

**Misc notes:**

* The black piece which acts to transfer the motion of the lower servo to the lower leg should be printed in two parts, then have a bearing inserted, then be glued together. There are configurations in Solidworks to allow the export of this but I will try add all STLs soon.
* All parts in contact with the motors MUST be printed in ABS for temperature resistance.
* PLA parts will soften due to the heat the motors produce (although this may be avoided using the fans). So all orange parts are ABS as well as the black hub which holds the servos for the upper and lower leg. (Note that the upper leg is in contact with the servos via the bolts which attach it so should also ideally be printed in ABS to avoid any issues)
* The rear upper and lower parts (large orange parts) that go aroudn the ports of the PI should be printed as a single piece. They were designed separate but you will get much better results just exporting the sub assembly as an STL and printing that
* All heat set inserts should be pushed in with a soldering iron tip.

### Wiring Diagrams

Use AWS12 wire for communications.  
Use AWG22-30 for any cables powering components.

For cable dimensions and where and how to buy it - refer to the bill of material file.   
Most of the wiring requires solder and a soldering iron.

#### Communications

![](https://media.printables.com/media/prints/1492731/rich_content/4251167d-1f1d-4012-a7a9-a2bcfef659ff/uploaded-image-wiring-diagram-communications-2.png#%7B%22uuid%22%3A%22f5cddf98-c842-4406-8075-74fade4bd3ad%22%2C%22w%22%3A660%2C%22h%22%3A403%7D)

#### Power

![](https://media.printables.com/media/prints/1492731/rich_content/7e41e53d-d3f6-4de6-9559-a0b271bff17f/uploaded-image-wiring-diagram-power-1.png#%7B%22uuid%22%3A%2278c09c74-57af-4c1b-99a7-802ef9d23e11%22%2C%22w%22%3A1050%2C%22h%22%3A587%7D)