# Car_Black_Box_Microcontroller_Project  
The Black Box, typically associated with airplanes, is crucial for analyzing incidents. Known as an Event Data Recorder (EDR) or Accident Data Recorder (ADR), it can also be installed in vehicles to record events like engine faults and speeding. This proactive monitoring ensures timely maintenance and improves safety. With password-protected access, transport managers can log critical activities, enhancing vehicle efficiency and tracking driver behavior. The system logs gear shifts, engine temperature, fuel consumption, and trip distance, aiding in proactive maintenance and better fleet management.

##Requirements:  

1. **Run Makefile in CBB_EEPROM_Loader Folder**:
    - Stores initial values in External EEPROM.

2. **Run Makefile in CBB_Main Folder**:
    - Starts execution on PIC18F4580 Micro-controller.
    - Uses an on-board CLCD screen for the interface.

3. **Dashboard Display**:
    - Shows current time, last event, and vehicle speed.
    - Speed adjustable via on-board POT.
    - Matrix SW1 for Gear UP, SW2 for Gear DOWN, SW3 for Collision.
    - Events stored in External EEPROM.

4. **Password Screen**:
    - Press Matrix SW8 to access.
    - Default password: "0000" (changeable).
    - Matrix SW8 for '0', SW9 for '1'.
    - Password input shows as '*'.
    - Log Menu access on correct password.
    - 5 attempts before a 60-second lockout.

5. **Log Menu Options**:
    - **View log**: Last 10 events from External EEPROM.
    - **Clear log**: Clears logs.
    - **Change Password**: Set new password.
    - **Download log**: Uses UART communication; data appears on Serial monitor.
    - Long press Matrix SW11 to navigate back to the Dashboard.

#Software Tools Used
- [1. MPLABxIDE](https://www.microchip.com/en-us/tools-resources/develop/mplab-x-ide)
- [2. MPLABxC8 Compiler](https://www.microchip.com/mplab/compilers)
- [3. PICSim Lab Simulator](https://www.picsimlab.com/)
