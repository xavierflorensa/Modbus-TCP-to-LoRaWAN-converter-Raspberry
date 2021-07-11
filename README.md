# Modbus-TCP-to-LoRaWAN-converter-Raspberry
This application uses this repository
https://github.com/pmanzoni/raspi-lmic
but modifying the file https://github.com/pmanzoni/raspi-lmic/tree/master/examples/ttn-otaa/ttn-otaa.cpp
to take the data to send from a file missatge.txt stored on same directory on Raspberry PI
as explained on the pdf
We use node-red running on the same raspberry as the Pi-HAT to get data from any Modbus-TCP device on register 0 and write on the file missatge.txt
Then the routine ttn-otaa.cpp takes the data from file and sends thru LoRaWAN
