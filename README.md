![Morlock-POS](https://user-images.githubusercontent.com/50764330/141025891-1816fd68-6cb5-4aaf-9084-d06c5fc7e6b1.png)
<br />
[![self](https://img.shields.io/badge/Morlock--POS-v1.3r3-purple)](https://github.com/VexisMorlock/Morlock-Pass/)
[![Raspberrypi](https://img.shields.io/badge/Raspberrypi-4B-9cf)](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/)
[![Python](https://img.shields.io/badge/Python-3.73-9cf)](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/)
[![PyQt](https://img.shields.io/badge/PyQt-5%20or%206-purple)](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/)



POS system using rfid, raspberrypi, python, and mysql

uploading working concept.  
## Change log:
- Added better more coherent comments
- Added real time clock (not included in code but, added hardware)
- Fixed issue with scaling on odd formatted tvs
* Added home buttons to all windows excluding teacher mode
	* not going to add unless clients feel like it's needed

## Future software  changes:
* Creat methods for massive GUI windows.
	* This wasn't done before because I didn't have time; school was starting.
- Modulate files so there's less clutter
* Get initial store/student information from database
	*I don't like that some of the info is hard-coded, this needs to be fixed and moved to a more friendly way of changing the items in the store.
	*Need to add a good way for the admin to add things into the store or take them away when they run out. 
* Improved UI
* Add in the option for non standard fines and bonuses
* Add feedback to bonus and fine windows when charging
	* Can lead to confusion if I don't let the admin know that the transaction is complete.  
## Future hardware changes:
* Need to redo wiring
	* I need to either design a hat to use or make my own cables to achieve a more finished look.
	* Clear plastic was not a great choice for a box.
* Add an option for a bigger lcd screen
	* It would give me more space to give customers more info at time of purchase
* Add rgb indicator led
	* Always good to give more feedback

## Equipment:
* Raspberrypi 4 
	* May not need something this fast for this project, but it helps with the user experience
* Micro sd card with Raspberrypi OS
* RC522 RFID Reader
* 16x2 LCD with full header (used non i2c for this but could be easy to adapt to)
* 10k Potentiometer
* Mouse
* Realtime clock with battery (not needed and software not included, but it helps if your project has no internet connection)
  
  
## Dependencies:
* Python 3.7 or higher
* Pip3
* Adafruit CharLCD library
* Raspberry Pi GPIO
* SPI enabled
* Spidev library
* MFRC522 library
* MYSQL server
* MYSQL connector for python
* PyQt5 or pyqt6 (configured for 5 follow notes for changing to version 6)
    
## Migrate to PyQT6:
- Change exec statements
	* exec_()  ---> exec()
		* You will need to do this for all exec statments, there is one for every window; all are commented and should be easy to find.
    
    
  
