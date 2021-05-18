MSR605 Magnetic Card Reader / Writer
  ------------------

_Edited: 18  May, 2021_

Authors:
- Liam Hogan - bentbot@outlook.com
- Manwinder Sidhu - manwindersapps@gmail.com

Platform: Windows / Mac
Python: 2.7.16
Legal Documentation: LICENSE

  Project Description
  -------------------
  Simple GUI for reading and writing to 3-striped magnetic cards with a MSR605 on a USB/serial interface. Forked from Manwinder's [original project](https://github.com/manwinder123/MSR605-Card-Reader-Writer-Eraser-with-GUI), this version uses an [alternative library](http://web.mit.edu/~achernya/Public/msr.py) to connect with the device.

  Requirements
  ------------------
  A MSR605 magnetic card reader / writer (or an equivilent device with a complete python library).
  One or more standard 3-stripe magnetic cards.
  Python 2.7+
  
  Libraries Required
  ------------------
  MSR Library [Damien Bobillot - damien.bobillot.2002+msr@m4x.org]
  Tkinter for the GUI [Manwinder Sidhu - manwindersapps@gmail.com]

  Installation & Run
  ------------------
      # Start the GUI
      python ./GUI.py

      # Install serial if needed
      pip install serial
 
      # Update the serial port line in ./GUI.py:20
      SERIAL_PORT = '/dev/cu.usbserial-142430'

  Hardware Description
  --------------------
  The MSR605 is a card reader/writer, its writes to the standard magstripe cards
  that most people are used to using (Credit Cards, Debit Cards, pretty much any
  card with a colored stripe on the back, its usually black). I purchased mine
  on ebay. I choose to buy this card reader because it had good documentation
  online

  File Description
  ----------------
  GUI.py - the graphical interface that allows you to control the MSR605
  msr.py - the library that connects to the card reader (MSR605)  

