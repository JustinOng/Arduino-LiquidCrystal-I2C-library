# 1602 LCD over Software I2C

This is a library meant for I2C LCDs but utilising software I2C for that rare case when your I2C bus is not available/does not exist.

[SlowSoftI2CMaster](https://github.com/felias-fogg/SlowSoftI2CMaster) is used to provide the software I2C master.

The only change made is to the class name and constructor, `LiquidCrystal_I2C` is now `LiquidCrystal_SWI2C`.

To initialise, use

    LiquidCrystal_SWI2C(uint8_t sda_pin, uint8_t scl_pin, uint8_t lcd_addr, uint8_t lcd_cols, uint8_t lcd_rows, uint8_t charsize = LCD_5x8DOTS)

Take a look at examples for more well, examples.

# Installation #
Create a new folder called "LiquidCrystal_I2C" under the folder named "libraries" in your Arduino sketchbook folder.
Create the folder "libraries" in case it does not exist yet. Place all the files in the "LiquidCrystal_I2C" folder.

# Usage #
To use the library in your own sketch, select it from *Sketch > Import Library*.

-------------------------------------------------------------------------------------------------------------------
This library is based on work done by DFROBOT (www.dfrobot.com).