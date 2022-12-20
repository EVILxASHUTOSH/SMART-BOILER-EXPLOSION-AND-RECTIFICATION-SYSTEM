# SMART-BOILER-EXPLOSION-AND-RECTIFICATION-SYSTEM
## TABLE OF CONTENT  
- About
- Working
- Software Implementation
- Hardware Implementation
- Usage
- Roadmap
- License
- Contact
## ABOUT
Every year there are several boiler explosion cases, and we designed a project that can solve this avertable accident. The project is focussed on getting various data required from the boiler and using that to analyse the possible threat, then accordingly the solution will be deployed. One of the classic mechanisms would be, when the temperature rises, our circuit will make the valve sending in fuel reduce the amount sent. Hence the temperature will reduce. 
This problem is avertable, because of the fact that there is no timely monitoring and alerting the concerned worker or people responsible for the control of the boiler. So, we have devised a strategy to solve this issue by tracking all the vital readings from a boiler and documenting it. Over a period of time, boiler operating logs help distinguish operating trends that can allow problems to be diagnosed, and boiler system maintenance to be scheduled, before an emergency shutdown is necessary. This problem is not only restricted to boiler plants, but any industrial application where there is a need for controlling the amount of input substance into a chamber and monitoring necessary parameters. So on a larger scale the same application could be taken and applied on to several other industrial applications that have similar functionality. 
 
## WORKING
Our project is mainly focused on getting sensor values of temperature and humidity and using those values , we control the servo motors. The servo motors are responsible for controlling the valve that opens and closes the fuel or any stored liquid based component being sent into the boiler. This can give an overall control over the hazard regulations of the boiler. The overall Simulation was done in Proteus, we connected all the sensors to the microcontroller, except the Pressure sensor the rest were digital sensors, therefore an analog to digital converter was connected to the pressure sensor so that the values are stored in the microcontroller. The real time values of the sensors are tracked and displayed in small intervals in the LCD display placed in the circuit. Overall the servo motors are made to rotate according to the amount of value difference shown in the sensors. If it goes above or below certain values, the servo motors are rotated in respective directions. 
 

Algorithm Structure of the System 
 
 
Project Block Diagram 

Presently, we use distributed control systems in the industries, using a panel control unit to control and monitor the temperature and flow parameters. Manual assistance at all times when the plant is in operation is the limitation of this system. The person who is present inside the plant during an emergency also is in risk of his/her life in case of any emergency. Hence, we propose a model so that the operating person can remotely control and monitor the boiler feed water in a power plant. Boiler parameters such as water level, pressure and temperature are monitored using water level sensor, pressure sensor and temperature sensor respectively. The real time information of these parameters will be sent to the programmed decision making microcontroller unit which will turn ON/Off corresponding parameter relays and its associated switching units depending upon the real time information received from the various parameter relays, if the operating conditions are well within the preset limits then no control command will be sent to the relay via the decision making microcontroller or else if there is any violation in the operating conditions then microcontroller will send the control signal to the associated relay to turn ON/OFF depending on the real time information. The real time information can be visualized on the LCD display and the same information can be sent to the mobile-phone registered number in the form of SMS via GSM 

## SOFTWARE IMPLEMENTATION

Proteus Circuit Diagram 
In this system transmitter section mainly consists of three sensor networks which senses various boiler parameters. Temperature sensor, PIR sensor and pressure sensor are used in this model. Sensors analog output are connected to ADC (Analog to Digital Converter) to convert analog information to digital form, then this digital information is processed using PIC 8051 microcontroller. PIC 8051 microcontroller does the controlling section. Whole sensor’s data are stored in the processor memory and sent to the database then to the display device. It indicates the workers through a buzzer in the workplace and through an alarming system in the user system by GSM receiver in remote places which have connectivity to the 8051 microcontroller if any of the sensor's data exceeds or below its threshold level. The connected servos are used to turn ON/OFF the fuel and water tank valves according to the situation. Hence we can automatically control the environment of the boiler. 

## HARDWARE IMPLEMENTATION

From both the simulation and the hardware implementation we could cover the objectives of the project. Even though the simulations provided trustworthy results, hardware implementations verifies all the simulation data and outputs. Simulations were conducted using Proteus software as shown in the figure given down below. Normal pressure indicates that the pressure inside the boiler is under safe limits. A lot of boiler explosion cases have been seen due to extreme pressure build up inside the boilers due to the steam produced by the fluids of the container. If the pressure exceeds the safe range which has been applied inside the code, an alarm of high pressure will be displayed 
 
 
Simulation Output under normal condition 
 
 
Simulation Output under emergency condition 

Flow Detection uses a PIR sensor which detects the movement of the fluids through pipes. This leakage can cause hazards not only to the workers but can be inflammable which will put the entire factory in danger. Therefore the PIR sensor notifies incase of any change in the fluid level or outflow of fluid even if it’s not needed. The temperature and humidity sensor is very important and notifies the real time value. Sometimes the rise in temperature causes the formation of steam of the fluids present inside the boilers. Two servo motors are also connected which will be activated in case of high temperature and high pressure. It has been added for safety which will eject excess pressure and excess fluids when the temperature rises due to any situation. The virtual terminal is added to replicate the GSM module which will give real time updates and emergency messages to the head of the factory or the owner who can take any actions required in the case of any emergency. Such systems are very important as seen after the unforgettable scenarios of Bhopal Gas Tragedy. 
In terms of the hardware demonstration of the system, pressure, temperature, humidity and PIR sensor was added in order to check the conditions of the simulations and was verified. The GSM module could not be added into the demonstration since there was no stock in the market. Apart from the GSM module, all the other connections have been checked and the working picture has been added in the figure below. 
 
 
Hardware Demonstration of the entire system 

In terms of hardware drawback, the servo is supposed to rotate when the temperature is more than the safe level which is set at 20C for demonstration purposes. But the power required by the servo cannot be provided by the 8051 development board and therefore even though the servo vibrates, it does not rotate the required angle. An external battery needs to be added in order to provide enough power to the servo. If attached to the board, it sometimes draws more power and makes the LCD flicker and not work properly. 

Complete Hardware System 



## ROADMAP
Even though our project is a miniature small scale replica of what can be done, we could use this exact same application at a larger scale and actually solve this extremely prevalent problem in the industry. The future prospects of the project range from publishing the outputs online to sending quick messages to factory workers as an alert. This problem is not only restricted to boiler plants, but any industrial application where there is a need for controlling the amount of input substance into a chamber and monitoring necessary parameters. So on a larger scale the same application could be taken and applied on to several other industrial applications that have similar functionality. By the integration of basic sensors and using them to calculate the parameter values we are reducing the costs, and also by fully rotating the servo motor without a control system application, we are further reducing the complexity and solving this problem in the most straightforward way possible. 


## License
Distributed under the MIT License. See LICENSE for more information.

## Contact
@EVILxASHUTOSH-dearashutoshmishra2002@gmail.com

Project link: https://github.com/EVILxASHUTOSH/SMART-BOILER-EXPLOSION-AND-RECTIFICATION-SYSTEM
