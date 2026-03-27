# Vibration Sensor (OrCAD PCB Design)

This repository contains the hardware design (Schematic Capture and PCB Layout) for a low-power impact and vibration sensor. It was developed as an academic CAD project.

## About the Circuit
The system is designed to detect physical impact or vibrations on surfaces. 
* **Detection:** A piezoelectric ceramic sensor detects the acceleration of the impact.
* **Signal Processing:** The raw signal is filtered by a capacitor and triggers an M74HC123 monostable multivibrator.
* **Output:** The monostable generates a pulse that drives an NPN transistor (BC547) into saturation. This open-collector output can be used to switch external devices like alarms.
* **Power:** The circuit is highly efficient, drawing only about 5-6 mA, and is powered by a standard 3V button cell battery.

## PCB Specifications
The printed circuit board was designed in OrCAD following these rules:
* **Layers:** 2 layers (TOP and BOTTOM).
* **Component Placement:** All components are Through-Hole Technology (THT) and placed on the TOP layer.
* **Routing:** Signal traces are routed at 0.3 mm; power traces are 1.1 mm wide.
* **Grounding:** The BOTTOM layer features a copper ground plane.

## Repository Structure
* 📂 `Design_Files/`: Contains the OrCAD source files (the .dsn schematic and the .brd PCB layout).
* 📂 `Manufacturing_Files/`: Contains the generated manufacturing files (Gerbers, NC Drill).
* 📂 `Datasheets/`: Datasheets for the main electronic components used.
* 📄 `BOM_Vibration_Detector.xlsx`: Detailed Bill of Materials.
* 📄 `Proiect_CAD-Vibration_Detector.pdf`: The complete project report (DRC, layout prints, conclusions).
