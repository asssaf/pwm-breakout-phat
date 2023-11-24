# pwm-breakout-phat
A pHAT for Raspberry Pi, breaking out the PWM pins and some proto area.

The PWM pins are broken out into four 3-pin connectors that can be used with 5V servos. Granted, it's not recommended to run a servo directly from the pi pins without any protection. 
But in practice, running micro servos (such as sg90), especially one at a time, should be ok (but do it at your own risk). 

In order to enable hardware PWM, the appropriate overlay needs to be enabled in `config.txt`. For example:
```
dtoverlay=pwm-2chan,pin=12,func=4,pin2=13,func2=4
```

The board also has a couple of STEMMA-QT connectors for I2C convenience.

This was my first attempt at designing a PCB in kicad.

## Schematic
![image](https://github.com/asssaf/pwm-breakout-phat/assets/445552/9c86cfea-85a6-4fbd-bb00-8d6bab838621)

## PCB
![breakout_front](https://github.com/asssaf/pwm-breakout-phat/assets/445552/b4fd969f-b086-45a4-8af5-0424d37bb7d2)
![breakout_back](https://github.com/asssaf/pwm-breakout-phat/assets/445552/71b862d1-e58b-4157-89b3-c7594aa0feab)



<img src="https://github.com/asssaf/pwm-breakout-phat/assets/445552/d1748a43-8422-45ef-a861-9130384fb440" width="510" />

<img src="https://github.com/asssaf/pwm-breakout-phat/assets/445552/fb6683cd-17f2-46c5-b49e-caedf715c5b0" width="512" />

![pwm](https://github.com/asssaf/pwm-breakout-phat/assets/445552/e8f5a4c9-7569-49a8-befb-26418d36b4ac)
