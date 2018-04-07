# A simple driver for IrDA remote Controler
------
##How to use it 
> * Init a PWM timmer channel(38Khz) and a internal clock timmer(for precise control).
> * copy this ropo to your project,select correct library file (such as stm32f1xx_hal.h).
> * edit the macro to yours,change timers to your init just now.
> * enjoy it!


##Some tips about IrDA
IrDA is a cheap, convenience remote method. it use NEC to control PWM to transmit data.
Normally, IrDA remote controler send a uint8_t data byte to set a command,and a uint8_t address byte to distinguish different device.