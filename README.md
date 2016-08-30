# ESP-Web-Server-v2

A web server built using the ESP8266 using the WEMOS D1 Mini to ease the build and assembly, but any ESP8266 would do.

The webserver uses files loaded from an SD Card - the WEMOS SD shield and controls the on-board LED, the WEMOS Relay shield and
displays images loaded from the card. There is a index page that controls the I/O functions.

The WEMOS DHT11 shield is used to display on a web page the current temperature and humidity. To do this, two examples are provided, one
uses the ESP8266 to read the DHT temperature and humidity, then adds an HTML wrapper, then directly serves the HTML to the client, in the
other the ESP8266 reads the temperature and humidity then writes the data to a text file on the SD Card, then uses HTML to construct
a web page around the values to be displayed, showing how values can be parsed between environments and used for data logging.

With the exception of the ESP8266 .ino file, copy all files to an SD Card, insert it to the SD Card reader, compile the code and the
server is ready.

In this version 2, a test web site is provided, which is ready for use allowing users to edit the contents for their own use, in addition
the ability to display SD card contents has been added and minor code improvements have been made.
