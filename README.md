MSR605 Magnetic Card Reader / Writer
  ------------------
_Edited: 21  May, 2021_
!['MSR605-GUI Screenshot on macOS Catalina'](https://raw.githubusercontent.com/bentbot/MSR605-GUI/master/MSR605-GUI.png)
### Download the Application:
- MacOS Catalina  - Version 1.0
    - MSR605 Card Reader Writer.app
    - [Download the Application (Zip - 60Kb)](https://github.com/bentbot/MSR605-GUI/blob/master/dist/MSR605CardReaderWriter.zip?raw=true)
- Windows: coming soon...
    - Compile it yourself with a .py to .exe tool!

### Project Description
  Simple GUI for reading and writing to 3-striped magnetic cards with a MSR605 on a USB/serial interface. Forked from Manwinder's [original project](https://github.com/manwinder123/MSR605-Card-Reader-Writer-Eraser-with-GUI), this version uses an [alternative library](http://web.mit.edu/~achernya/Public/msr.py) to connect with the device.

###  Requirements
  A MSR605 magnetic card reader / writer (or an equivilent device with a complete python library).
  One or more standard 3-stripe magnetic cards.
  Python 2.7+
  
###  Libraries Required
  MSR Library [Damien Bobillot - damien.bobillot.2002+msr@m4x.org]
  Tkinter for the GUI [Manwinder Sidhu - manwindersapps@gmail.com]

###  Installation & Run

      # Start the GUI
      python ./MSR605 Card Reader Writer.py

      # Install the serial module if needed
      pip install serial
 
      # Update the serial port:
      #./MSR605 Card Reader Writer.py:20
      SERIAL_PORT = '/dev/cu.usbserial-142430'
###  Build From Source
      # Install the build tools
      pip install -U py2app
      
      # Build application package from source
      python setup.py py2app -A
###  Hardware Description
  The MSR605 is a card reader/writer, its writes to the standard magstripe cards that most people are used to using (Credit Cards, Debit Cards, pretty much any card with a colored stripe on the back, its usually black). I purchased mine on ebay. I choose to buy this card reader because it had good documentation online.

###  File Description
 - ./MSR605 Card Reader Writer.py 
    - The graphical user interface source.
 - ./msr.py 
    - The library that connects to the card reader (MSR605).
 - /dist/MSR605CardReaderWriter.zip 
    - The compiled application (.app) package for download.

### Authors
- Liam Hogan
    bentbot@outlook.com
- Manwinder Sidhu
    manwindersapps@gmail.com
