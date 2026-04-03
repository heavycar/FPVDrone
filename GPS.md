so i decided to add a gps module to the build, it's not really necessary for basic flying but it adds some really useful features like return to home and position tracking

basically it lets the drone know where it is in real time, which is important in case something goes wrong or if i just want to know how far i went

it connects to the flight controller using a uart, so nothing too complicated

i still need to configure it in betaflight later, but for now it's just part of the plan

i want to use a Beitian BN-880 cuz it comes with integrated compass, strong signal and it's widely used on FPV world, it' really not that expensive and simple to set up
here are some nerd info dumping🤓☝🏼

 Chip: u-blox M8N
- GPS + Compass (HMC5883L / QMC5883)
- Comunication: UART
- Voltage: 5V
- it can add some good functionalities like return-to home and map 

![shopping](https://github.com/user-attachments/assets/c9c8a4ad-ccf3-4ba7-b678-76c7c8c43bec)
