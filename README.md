# USB-OTG Maker

## Overview
This example was originally developed in the iPP4CPPS project. The model simulates a production line for USB-OTG sticks, which was chosen as a representative plant that might potentially be expanded into a full production line.

![Layout of the simulated production line, as depicted in the Unity rendering (left), and the physical demo stand (right), containing: 1) the Warehouse stacks; 2) the assembly box at the base of the Warehouse stacks; 3) the memory boxes of the Warehouse unit; 4) the robotic arm for moving parts around the Warehouse; 5) wagons on different locations of the track; 6) the loading station; 7) the test station; 8) the circular track for the wagons.](resources/Layout.png)

*Figure: Layout of the simulated production line, as depicted in the Unity rendering (left), and the physical demo stand (right), containing: 1) the Warehouse stacks; 2) the assembly box at the base of the Warehouse stacks; 3) the memory boxes of the Warehouse unit; 4) the robotic arm for moving parts around the Warehouse; 5) wagons on different locations of the track; 6) the loading station; 7) the test station; 8) the circular track for the wagons.*

The USB-OTG sticks chosen consist of three parts (two lids and the main body). The production line reads orders from a CSV file, and shoul be able to respond properly to changes in requests / cancellations and assemble a stick with the required characteristics from parts available in a warehouse. The completed product should then move on a conveyor system to a test station, which validates the component before passing the completed product to the user. If the item is rejected (the test fails to confirm the requested colours on the stick), then the process is automatically re-started and a new request is made to the warehouse.


## Supported Features
This study supports the following INTO-CPS technologies:

* Overture VDM-RT models (and FMUs)
* INTO-CPS SysML  
* Co-simulation Engine (COE)
* Code Generation

## Additional Information
The VDM-RT FMUs have been gradually replaced during the development project with 20SIM and 4DIAC FMUs. However, because they have been developed by the industrial partners, they could not be included in the example. Also, for the physical model, code generation allowed the deployment on Raspberry-Pi driven components. Additional Information about this case study can be found in the INTO-CPS-Manifesto (Manufacturing case study).