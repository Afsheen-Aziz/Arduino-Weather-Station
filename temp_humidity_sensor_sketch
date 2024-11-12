
//Libraries

#include <DHT.h>


//Constants

#define DHTPIN A3     // what pin we're connected to

#define DHTTYPE DHT11   // DHT 11

DHT dht(DHTPIN, DHTTYPE); //// Initialize DHT sensor for normal 16mhz Arduino



//Variables

//int chk;

int h;  //Stores humidity value

int t; //Stores temperature value



void setup()

{

    Serial.begin(9600);

    Serial.println("Temperature and Humidity Sensor ");

    dht.begin();
    

}



void loop()

{

    //Read data and store it to variables h (humidity) and t (temperature)

    // Reading temperature or humidity takes about 250 milliseconds!

    h = dht.readHumidity();

    t = dht.readTemperature();

    

    //Print temp and humidity values to serial monitor

    Serial.print("Humidity: ");

    Serial.print(h);

    Serial.print(" %, Temp: ");

    Serial.print(t);

    Serial.println(" ° Celsius");


  delay(2000); 

}

