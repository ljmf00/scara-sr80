# Digital Interfaces

## X6/RS232 -10V/+10V
- **Type:** 9 pin sub-D connector, female
- **Location:** Front panel of the controller T161-90x

![X6 Interface on Moog Front Panel](../assets/moog/front_servo.jpg)

### Pinout
|Pin assignment|Description|Input/Output|
|---|---|---|
|1|Not Connected||
|2|RX Read Data Input|Input|
|3|TX Transfer Data Output|Output|
|4|Not Connected||
|5|Digital Ground|I/O Reference |
|6|Protective Earth|I/O Reference |
|7|Not Connected||
|8|Not Connected||
|9|+5V Output Supply Voltage|Output|

### Communication Settings
- **Baudrate:** 9600
- **Startbits:** 1
- **Databits:** 7
- **Paritybit:** ignored
- **Stopbits:** 2

***NOTE:*** This interface signal swing from -10 to +10V. To convert this signal to TTL (0V to +5V) you need to use a MAX232 IC.

![RS232 to TTL using MAX232 Pinout](../assets/rs232_max232_pinout.png)

![MAX232 on a breadboard](../assets/rs232_ttl.jpg)

## X6/RS485/CAN
- **Type:** 9 pin sub-D connector, male
- **Location:** Backplane

![X6 RS485 CAN Interface on Back](../assets/can/back.jpg)
![CAN Interface on Front](../assets/can/front.jpg)

### Pinout
|Pin assignment|Description|Input/Output|
|---|---|---|
|1|Digital Serial Input/Output (Option)||
|2|Digital Serial Input/Output (Option)||
|3|RS485 Bus Interface, Plus|I/O|
|4|RS485 Bus Interface, Minus|I/O|
|5|???||
|6|Protective Earth|I/O Reference |
|7|Not Connected ???|I/O Reference |
|8|Not Connected||
|9|Not Connected||