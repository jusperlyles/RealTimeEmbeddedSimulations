find it at https://www.tinkercad.com/things/bFzYkZyC6kG-neat-turing/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits&sharecode=rldnZpdnwTX3xAeLtWQJwCCzTM4DocR72Zw-kd_bPF0,


1. System Overview
This project involves designing an embedded system to secure restricted areas by monitoring entry points and internal movement. It distinguishes between normal operation (door closed) and high-security alerts (door open with internal movement).


3. Core Components
Microcontroller (Arduino Uno): Serves as the central processing unit, executing the security logic and managing input/output signals.
Door Sensor (Micro Switch): A mechanical switch used to detect the physical state (open or closed) of the door.
Motion Sensor (PIR Sensor): A Passive Infrared sensor that detects movement by sensing changes in infrared radiation emitted by people.
Output Indicators:
Green LED: Indicates "Normal" or "Secure" status when the door is closed.
Red LED: Indicates an "Alarm" state when an intrusion is detected.
Piezo Buzzer: Provides an audible siren during an alarm event. 


4. Working Logic
The system operates on three primary logical conditions: 
Normal Condition: When the door is Closed, the Green LED remains ON to indicate a secure state.
Alarm Condition: If the door is Open and the PIR sensor simultaneously detects motion, the Red LED flashes and the Buzzer sounds to alert of an intruder.
Standby/Idle: If the door is open but no motion is detected, indicators remain OFF (or the system waits for movement). 


5. Key Features & Advantages
Real-time Monitoring: Provides instant feedback on security breaches via physical indicators and serial monitoring.
Cost-Effective: Utilizes affordable, widely available sensors and microcontrollers.
Scalability: Can be expanded to include GSM modules for SMS alerts or IoT connectivity for remote smartphone notifications. 


6. Debugging & Maintenance
Stabilization: PIR sensors typically require a 15–60 second warm-up period to stabilize their baseline infrared reading.
Pull-up Resistors: Using INPUT_PULLUP on the Arduino ensures a stable high signal when the door switch is open, preventing false triggers from electrical noise.
Serial Debugging: The Serial Monitor in the Arduino IDE is used during development to verify sensor readings in real-time. 

YouTube
 +2
