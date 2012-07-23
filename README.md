PHP-Emoncms-Serial-Link-
========================

WORK IN PROGRESS!

A PHP scrip to run on a Raspberry Pi to receive serial data from a JeeLink running RFM12B demo, decode the RFM12B packets and post to emoncms. 

Support decoding the RFM12B packets into integers adding multiple modes and posting to emoncms using new CSV format. Naming of nodes and variables is done on emoncms. 
Possibly this could be integrated into emoncms in the future...

To have the script run in the background as a deamon, I use “sudo nohup php serial.php &”. To stop it, you must find the processID with “ps -A” and “kill” it.

------------------------------------------------------------------------------

Based on and inspired by the great work by Martin Harizanov: 
http://harizanov.com/2012/06/capture-decode-and-log-to-emoncms-rfm12b-packets-on-raspberry-pi/

For JeeLink running RFM12B demo included in JeeLib library: github.com/jcw/jeelib

Used PHP serial from: http://code.google.com/p/php-serial/

Data structure of RFM12B packets: http://jeelabs.org/2010/12/07/binary-packet-decoding/
