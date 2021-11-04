# Morlock-POS
POS system using rfid, raspberrypi, python, and mysql

 Version 1.3 r2

uploading working concept.  
Change log:
	Added better more coherent comments
	*added real time clock (not included in code but added hardware)
	Fixed issue with scaling on odd formatted tvs
	Added home buttons to all windows excluding teacher mode
		not going to add unless clients feel like its needed
	

Future software  changes:
	Separate out files so less clutter
	Get initial store information from database
		I don't like that some of the info is hard-coded this needs to be fixed and moved to a more friendly way of changing the items in the store
	Need to add a good way for the admin to add things into the store or take them away when they run out 
	Improved UI
		It still kinda looks like a 90 website and I want to improve the look.
	add in the option for non standard fines and bonuses
		some may find this feature useful when handling issues where kids are doing some that needs a fine/punishment where it is not an enumerated incident
	Add feedback to bonus and fine windows when charging
		can lead to confusion if I don't let the admin know that everything went ok.  
Future hardware changes:
	need to redo wiring
		it looks super messy. I need to either design a hat to use or make my own cables.
		clear plastic was not a great choice for box
	maybe add a bigger lcd
		it would give me more space to give customers more info at time of purchase
	add rgb indicator led
		always good to give more feedback

Equipment:
  Raspberrypi 4 
    may not need something this fast for this project but it help with the user experienc
  Micro sd card with Raspberrypi OS
  RC522 RFID Reader
  16x2 LCD with full header (used non i2c for this but could be easy to adapt to)
  10k Potentiometer
  mouse
  realtime clock with battery( not needed and software not included but it helps if your project has no internet connection)
  
  
  Dependencies:
    python 3.7 or higher
    pip3
    Adafruit CharLCD library
    Raspberry Pi GPIO
    SPI enabled
    spidev library
    MFRC522 library
    MYSQL server
    MYSQL connector for python
    pyqt5 or pyqt6 (configured for 5 follow notes for changing to version 6)
    
Migrate to PyQT6:
  Change exec statements
    exec_()  ---> exec()
    you will need to do this for all exec statments there is one for every window; all are commented should be easy to find
    
    
  
