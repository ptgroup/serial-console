# Serial terminal
This is a simple serial terminal written in LabVIEW for easy interface with serial devices.
Select the serial port, type a command in the box, and press enter to send it to the device.
Note: you can use the up and down arrows on the keyboard to scroll back and forward in your command history.

## Configuration
You can configure the baud rate, as well as the line ending character (which will be used to terminate any data you transmit).
You can also convert special characters to more readable values (enabled by default):
any non-printable character in RX will be converted to the form {xx} where xx is the ASCII code of the character in hexadecimal,
and any character of the form {xx} in TX will be converted to the equivalent ASCII character before transmitting.
Any other characters (including malformed {specifiers}) will be transmitted verbatim.
