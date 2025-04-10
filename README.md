# **Control egg incubator temperature by PID**
# **Introduction**
This is project about the STM32F103C8T6 microcontroller, measure the incubator temperature and use the PID controller to calculate the PWM level, thereby controlling the amount of heat emitted from the light bulb to stabilize the temperature at the desired level. It has all the functions of a thermostat including:
- Microcontroller: STM32F103C8T6.
- Use PID algorithm to adjust temperature (heat emitted from incandescent light bulbs)
- Use the push button to increase or decrease the temperature (using External interrupt)
- LCD screen to display temperature
- Collect temperature using DHT22 sensor
## Knowledge used in the project

- Uses HAL library and STM32CubeMX software
- Use timer1 to create a delayus function that communicates with DHT22
- Use timer2 to hash the PWM pulse to adjust the brightness of the heat-generating bulb
- Use timer3 as update time in PID controller
- Uses I2C communication standard to communicate with LCD screen
- Use an external interrupt as an input to control the temperature increase or decrease for the push button

## Result

Image displayed on LCD when temperature reaches setpoint and fluctuates stably with error 0.1 - 0.2°C  
(The setpoint in the project is set to 37°C)

![image](https://github.com/user-attachments/assets/b4a5feb5-d683-487f-a1de-2b22da7e35d6)

Overview image when setting up the project

![image](https://github.com/user-attachments/assets/6990807c-3b0e-40c9-842c-ad4126f4ccb9)


