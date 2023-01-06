# Temperature and humidity sensing with firebase storage

## INTRODUCTION
> Temprature and Humidity is sensed using a DHT11 sensor and the data is sent to Firebase for storage and a webapp is used to display the data. The project is based on temperature and humidity monitoring of environment. This project aims at the environments where air conditions might be extreme or need to be controlled. Humidity and Temperature are of importance when considered together and are quite crucial to many industries. Level of humidity not only affects individuals but also affects manufacturing processes, or storage in the industry. For examples, in semiconductor industry moisture level need to be controlled properly to ensure wafer processing. Humidity and Temperature monitoring is also important in incubators, respiratory equipment and biological products. Such type of systems constantly monitor environment and generate alerts if the parameters being recorded exceed a certain threshold.

## OUTCOMES
> Temperature monitoring system are versatile and hence can prove to be very efficient in keeping the environment controlled and stable. They aid in saving time, thereby increasing productivity, maintain regulatory compliance, hence increasing the quality of products. It is expected that the monitoring system achieves the following outcomes: 

* Continuously monitor the environment for humidity and temperature conditions
* Generate alerts if the present conditions reach or exceed a certain threshold
* Operate in such a manner to ensure quality of products being stored hence saving cost and effort

## Specifications
* 3 to 5V power and I/O
* 2.5mA max current use during conversion (while requesting data)
* Good for 20-80% humidity readings with 5% accuracy
* Good for 0-50 °C temperature readings +-2 °C accuracy
* No more than 1 Hz sampling rate (once every second)
* Body size 15.5mm x 12mm x 5.5mm
* 4 pins with 0.1" spacing
* Adafruit Learning Documentation for DHTxx Sensors
* RoHS compliant

## TOOLS USED
* Arduino IDE
* Firebase Database

## Libraries
* ESP8266.WiFi.h – for wifi configuration
* Adafruit_Sensor.h – for DHT11 configuration
* DHT.h library – for DHT11 configuration
* FirebaseESP8266.h – for firebase data storage configuration

## Configuration 
As mentioned above DHT11 was connected to NodeMCU through data pin, here is the
detail of how the NodeMCU was configured to connect to the WiFi as well as
programmed.
1. NodeMCU driver and Arduino IDE were downloaded.
2. ESP8266 NodeMCU was configured in the Arduino IDE.
3. Related packages and libraries were installed.
4. To connect to the Wi-Fi, ESP8266.WiFi library was used. ESP was connected to our WiFi networking by provided the ssid and password.
const char* ssid = "YOUR WIFI NETWORK NAME";
const char* password = "YOUR WIFI PASSWARD";
5. Similarly, database was configured using the FirebaseESP8266 library, and providing
the database URL as well as the authentication key.


## Web Interface

# going to add pics

## Statistical Evaluation
# Pic goes here
> The maximum temperature of the room was 29 degrees, which was when we turned on the room heater. The minimum temperature was observed to be 9.8 degrees, which during the night. The average temperature throughout the day was 20.3 degrees, which is because the heater was on throughout the day. Standard deviation was observed to be only 2.01 which might be due to the reason, because the sensor was placed in a confined environment. Maximum humidity is when we blew air on the sensor for testing. The average humidity is 18.33% which concludes that temperature was not humid throughout the day, and there was only a small variation of 4.8% during the day.

## Correlation
# pic goes here
> The correlation between temperature and humidity is inverse and is close to zero. This leads to the
conclusion temperature and humidity are not related.