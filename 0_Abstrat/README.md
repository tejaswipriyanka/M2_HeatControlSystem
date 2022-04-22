
## Heat Control System 

### Theory

The primary function of the heat control system is to regulate the temperature of a car seat. The button sensor is engaged when a user or driver of the car sits in the vehicle. The user then has the ability to turn on the heating. The temperature sensor continuously measures the temperature and transmits the analogue value to the microcontroller. The temperature sensor's analogue input is processed by the microcontroller, which then produces a temperature reading via serial connection. The control system's whole operation is controlled by an Atmega328 microprocessor.
### Simulation

The heat control system's functionality is coded in embedded C, and its operation is illustrated using SimulIDE simulation software.
The first image depicts the status of the simulation while the system is turned off, while the second image shows the status of the system when it is turned on.
#### ON
![ON](https://github.com/tejaswipriyanka/M2_HeatControlSystem/blob/main/6_Output/Simulation_ON.PNG)

#### OFF
![OFF](https://github.com/tejaswipriyanka/M2_HeatControlSystem/blob/main/6_Output/Simulation_OFF.PNG)

#### Outputs

|Circuit|RAM Table|
|:--:|:--:|
|![CIRCUIT](https://github.com/tejaswipriyanka/M2_HeatControlSystem/blob/main/6_Output/Circuit.gif)|!
[RAM_TABLE](https://github.com/tejaswipriyanka/M2_HeatControlSystem/blob/main/6_Output/RAM_table.gif)|
|CRO|Serial Monitor|
|![CRO](https://github.com/tejaswipriyanka/M2_HeatControlSystem/blob/main/6_Output/Oscilloscope.gif)|![ON](https://github.com/tejaswipriyanka/M2_HeatControlSystem/blob/main/6_Output/Serial_Monitor.gif)|

### Functionality 

* The first LED illuminates when the two switches are closed, signalling that the system and heater have been activated.
* The temperature sensor's analogue input is then received and digitised.
* The digitized temperature input is visualized using Pulse Width Modulation.
* The UART protocol transmits the corresponding temperature data based on the digital temperature input. The data is presented on the serial monitor in this location.
