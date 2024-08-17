![GIF-240817_172957](https://github.com/user-attachments/assets/23826bc5-9879-4eb0-b956-f8dbbc47afac)


### Digital Clock Using ATmega16

This project involves creating a simple digital clock using the ATmega16 microcontroller and a seven-segment display. The clock displays minutes and seconds, with buttons for setting and adjusting the time.

#### Key Components:
- ATmega16: Handles timekeeping and user inputs.
- Seven-Segment Display: Shows the time.
- Push Buttons: Five buttons (up, down, min, hr, enter) allow time adjustment.

#### How It Works:
1. Initialization: The microcontroller sets up the input/output pins and initializes the display.
2. Timekeeping Loop: The clock continuously updates and displays the time, incrementing the seconds every 100 loop cycles.
3. Time Setting: 
   - Press min or hr to enter time-setting mode.
   - Use up and down to adjust the time.
   - Press enter to confirm.

#### Code Highlights:
- `digitselect_def()`: Refreshes the display.
- `minute_def()` and `hour_def()`: Update the display based on the current time.
- `setclockmin()` and `setclockhour()`: Handle user input for setting minutes and hours.
  
#### Simulation:
A Proteus simulation file is included with this project, allowing you to test and visualize the clock's functionality before implementation.

#### Customization:
The clock is currently set to display minutes and seconds. To change it to display hours and minutes, modify the delay counter (delayCnt) logic in the main loop.

#### Important Note:
The clock might not be perfectly accurate due to potential timing drift. To improve punctuality, consider adding an external crystal oscillator to stabilize the clock frequency.

