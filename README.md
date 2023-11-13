# pwm-breakout-phat
A pHAT for Raspberry Pi, breaking out the PWM pins and some proto area.

The PWM pins are broken out into four 3-pin connectors that can be used with 5V servos. Granted, it's not recommended to run a servo directly from the pi pins without any protection. 
But in practice, running micro servos (such as sg90), especially one at a time, should be ok (but do it at your own risk). 
In order to enable hardware PWM, the appropriate overlay needs to be enabled in config.txt.

The board also has a couple of STEMMA-QT connectors for I2C convenience.
