# RyanPortfolio
Ryan Clark's Engineering Portfolio


## In - Space Metal 3D Printing
During my Master's I worked in the Future Manufacturing Reserach Lab at ASU. This lab developed a room-temperature metal 3D Printer using Resonance-Assisted Deposition. (https://www.padtinc.com/digital-manufacturing/glossary/resonance-assisted-deposition/)
<img width="1914" height="1436" alt="image" src="https://github.com/user-attachments/assets/5b686937-1a0a-4440-a69b-181b7a6524bc" />
<img width="1367" height="1821" alt="image" src="https://github.com/user-attachments/assets/1432a1e7-478c-4042-b850-c9ef95876f84" />

Room temperature (or low temperature) metal printing is ideal for use in space, where power usage and heat are both challenges. As part of a 2027 science package to the International Space Station, we began preparing the device for use in space. My role was adding additional sensing capability, specifically a load cell, to gauge manufacturing performance remotely. 

I integrated a force sensor with the CNC Control board to obtain precise force data coupled with toolhead position. To do this, I used an ESP32 to collect load cell data. This data was sent over Serial UART to a Raspberry PI. With some program modifications to the CNC control board, it sent toolhead position data using SPI to the raspberry PI, where the data was collated and stored.  
<img width="1905" height="1065" alt="image" src="https://github.com/user-attachments/assets/5126aebd-3feb-4726-aab5-4a83ee93283c" />



## Laser FF 3D Printer - GCode Post Processor
Also in the Future Manufacturing Research lab, and as part of my Python final project, I supported a Laser-FFF 3D Printer. This printer functioned much like a traditional 3D printer with a plastic filament, but it also utilized a laser, that heated the already deposited plastic in order to improve multi-axial strength and surface finish.
<img width="1535" height="1020" alt="image" src="https://github.com/user-attachments/assets/911d56ab-6c12-416e-b9e4-6fb53c040438" />

To support this project, I developed a custom extension for Cura, a 3D Printer tool that creates motion paths from a 3D Model. My extension took the traditional GCode output by Cura, then calculated and added laser positions to allow the laser to either be in line with or perpinidcular to the direction of motion. The extension then converted the laser-FFF GCode into an animated preview, to ensure the laser behaves as expected.
Cura:
<img width="2450" height="1220" alt="image" src="https://github.com/user-attachments/assets/cc791e78-c195-4476-8734-ac58e15bd8fb" />
Preview:
<img width="1350" height="1055" alt="image" src="https://github.com/user-attachments/assets/ec90244f-9b49-426a-833c-aaa6b7366b80" />


A video detailing the project:
https://www.youtube.com/watch?v=7vI6lZpDN5w 

Han, P.;  Riyad, M F.; Torabnia, S.; Clark, R.; Fonseca, N.; Hsu, K. (2025). In-process laser heating for surface finishing of carbon fiber reinforced nylon in fused filament fabrication. Journal of Reinforced Plastics and Composites


## Carbon Capture Impulse Sealer
The ASU Carbon Capture Lab hired a friend and I to automate a solution to their manufacturing process. As part of the carbon capture process, they filled fabric tubes with carbon-capture substrate. This substrate was then submerged underwater, where the carbon was released and fed to algae. These fabric tubes were made by hand using an [Impulse Sealer](https://m.media-amazon.com/images/I/71I5-QR3-oS.jpg), and the tubes had to be made precisely. Here is an example of the fabric tubes before they are filled:
<img width="1367" height="1823" alt="image" src="https://github.com/user-attachments/assets/2cc65e84-a926-49e1-b3a0-b9029d172a06" />


We came up with this solution:


