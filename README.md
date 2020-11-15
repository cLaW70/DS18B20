# DS18B20

int DS18B20_pin=2; 
DS18B20 DS18B20_sensor; 
 
void setup(){
  lcd.begin();
  lcd.backlight();
}
 
void loop(){  
 
  
  lcd.setCursor(0,1);
  lcd.print("Sicaklik:");
  lcd.setCursor(9,1);
  lcd.print((float)DS18B20_sensor.temperature, 2);   
   
  
  delay(1000);
 }
