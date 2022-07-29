# Photovoltaic-DC-motor-system-SM

Supplementary material openly available from the open access article:
Guerrero-Ramirez E., Martinez-Barbosa A., Contreras-Ordaz M.A., Guerrero-Ramirez G., Barahona-Avalos J.L. and Adam-Medina M. DC Motor Drive Powered by Solar Photovoltaic Energy: A FPGA-based Active Disturbance Rejection Control Approach. Energies 2022.

----------------------------------------------------------------------------------------------
This repository contains one simulation project and one implementation project.
----------------------------------------------------------------------------------------------
Software used:
-Matlab 2012b
-Xilinx ISE Design Suite 14.5 with Xilinx System Generator (XSG).
----------------------------------------------------------------------------------------------
Both projects are focused on the Nexys 4 development board with an Artix-7 100T FPGA.
It is worth mentioning that most of the texts inside the files are in Spanish.
----------------------------------------------------------------------------------------------
Simulation project:
-This is a Matlab/simulink simulation of the system: photovoltaic cells + SEPIC converter + Buck converter + DC motor.
-Upload the additional file (.mat) to the Matlab workspace because it is used to simulate the photovoltaic cells.
-The simulation uses XSG blocks for the control stage and simulink blocks for the power stage.

---------------------------------------------------------------------------------------------
Implementation project:
-This project contains a Matlab/Simulink file. This file contains all the control part of the system to be implemented on the Nexys 4 development board. The other files are VHDL codes for the operation of the ADCs and DACs, which are used in the Simulink file.
- With the simulink file, ISE Design suite projects are created and any other such projects are used for the FPGA. In this case 3 examples of projects created with different speed references are shown.
- Finally, the IOSTANDARD file is included manually in each project because the XSG version did not include the 3.3V standard in the terminals.
