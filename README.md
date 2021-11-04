# Morlock-POS
POS system using rfid, raspberrypi, python, and mysql


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
    
    
  
