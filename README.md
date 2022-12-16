# SPI_CONTROLLER

SPI_CONTROLLER

The Serial Peripheral Interface (SPI) is a synchronous serial communication interface specification used for short-distance communication. 
It uses separate clock and data lines, along with a select line to choose the device you wish to talk to.


![image](https://user-images.githubusercontent.com/120705715/208041578-271ca175-5d27-4532-a6ef-c0fd030ea168.png)

4-wire SPI devices have four signals:

Clock (SPI CLK, SCLK)
Chip select (CS)
master  out slave in (MOSI)
master in, slave out (MISO)

Data Transmission
To begin SPI communication, the main must send the clock signal and select the subnode by enabling the CS signal. 
Usually chip select is an active low signal; hence, the main must send a logic 0 on this signal to select the subnode. 
SPI is a full-duplex interface; both main and subnode can send data at the same time via the MOSI and MISO lines respectively. 
During SPI communication, the data is simultaneously transmitted (shifted out serially onto the MOSI bus) and received (the data on the bus (MISO) 
is sampled or read in). The serial clock edge synchronizes the shifting and sampling of the data. 
The SPI interface provides the user with flexibility to select the rising or falling edge of the clock to sample and/or shift the data

Results :
![spi_waveforms](https://user-images.githubusercontent.com/120705715/208041900-d59d154f-fbe5-4ada-a157-239910964e68.PNG)
