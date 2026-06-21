# RyanPortfolio
Ryan Clark's Engineering Portfolio


## In - Space Metal 3D Printing
During my Master's I worked in the Future Manufacturing Reserach Lab at ASU. This lab developed a room-temperature metal 3D Printer using Resonance-Assisted Deposition. (https://www.padtinc.com/digital-manufacturing/glossary/resonance-assisted-deposition/)
<p align="center">
<img height="400px"  alt="Mini-RAD Printer" src="https://github.com/user-attachments/assets/5b686937-1a0a-4440-a69b-181b7a6524bc" />
<img height="400px"  alt="Sample Part" src="https://github.com/user-attachments/assets/1432a1e7-478c-4042-b850-c9ef95876f84" />
</p>
Room temperature (or low temperature) metal printing is ideal for use in space, where power usage and heat are both challenges. As part of a 2027 science package to the International Space Station, we began preparing the device for use in space. My role was adding additional sensing capability, specifically a load cell, to gauge manufacturing performance remotely. 

I integrated a force sensor with the CNC Control board to obtain precise force data coupled with toolhead position. To do this, I used an ESP32 to collect load cell data. This data was sent over Serial UART to a Raspberry PI. With some program modifications to the CNC control board, it sent toolhead position data using SPI to the raspberry PI, where the data was collated and stored.  
<p align="center">
<img width="40%" alt="Block Diagram and Sample Data" src="https://github.com/user-attachments/assets/5126aebd-3feb-4726-aab5-4a83ee93283c" />
</p>


## Laser FF 3D Printer - GCode Post Processor
Also in the Future Manufacturing Research lab, and as part of my Python final project, I supported a Laser-FFF 3D Printer. This printer functioned much like a traditional 3D printer with a plastic filament, but it also utilized a laser, that heated the already deposited plastic in order to improve multi-axial strength and surface finish.
<p align="center">
<img width="40%" alt="Laser-FFF Process" src="https://github.com/user-attachments/assets/911d56ab-6c12-416e-b9e4-6fb53c040438" />
</p>
To support this project, I developed a custom extension for Cura, a 3D Printer tool that creates motion paths from a 3D Model. My extension took the traditional GCode output by Cura, then calculated and added laser positions to allow the laser to either be in line with or perpinidcular to the direction of motion. The extension then converted the laser-FFF GCode into an animated preview, to ensure the laser behaves as expected.                  
<p align="center">
<img width="45%" alt="Cura 3D Preview" src="https://github.com/user-attachments/assets/cc791e78-c195-4476-8734-ac58e15bd8fb" />
<img width="45%" alt="Custom Renderer" src="https://github.com/user-attachments/assets/ec90244f-9b49-426a-833c-aaa6b7366b80" />
</p>


Han, P.;  Riyad, M F.; Torabnia, S.; Clark, R.; Fonseca, N.; Hsu, K. (2025). In-process laser heating for surface finishing of carbon fiber reinforced nylon in fused filament fabrication. Journal of Reinforced Plastics and Composites


## Carbon Capture Impulse Sealer
The ASU Carbon Capture Lab hired a friend and I to automate a solution to their manufacturing process. As part of the carbon capture process, they filled fabric tubes with carbon-capture substrate. This substrate was then submerged underwater, where the carbon was released and fed to algae. These fabric tubes were made by hand using an [Impulse Sealer](https://m.media-amazon.com/images/I/71I5-QR3-oS.jpg), and the tubes had to be made precisely. Here is an example of the fabric tubes before they are filled:
<p align="center">
<img width="45%" alt="Fabric Tube Sample" src="https://github.com/user-attachments/assets/2cc65e84-a926-49e1-b3a0-b9029d172a06" />
</p>

We came up with this solution:
<p align="center">
<img width="40%" height="1821" alt="image" src="https://github.com/user-attachments/assets/dd4b7712-b115-49ab-b563-ec3e76f6f265" />
</p>

