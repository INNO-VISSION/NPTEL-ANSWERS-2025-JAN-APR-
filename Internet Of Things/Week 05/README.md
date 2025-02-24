#### Week 5: Introduction To Internet Of Things

##### *1. Which of the following is/are current challenges in IoT?*  
- A. Large scale of co-operation  
- B. Global heterogeneity  
- C. Both (a) and (b)  
- D. Neither (a) nor (b)  
*Answer:* C. Both (a) and (b)  
*Explanation:* IoT faces challenges like large-scale device cooperation and global heterogeneity, where devices use different protocols and standards.  

---

##### *2. Interoperability is not a characteristic of a product or system.*  
- A. True  
- B. False  
*Answer:* B. False  
*Explanation:* Interoperability is a key characteristic of IoT systems, allowing devices to communicate and work together despite differences.  

---

##### *3. Interoperability is required because:*  
- A. There are different programming languages  
- B. There are different communication protocols  
- C. Both (a) and (b)  
- D. Neither (a) nor (b)  
*Answer:* C. Both (a) and (b)  
*Explanation:* IoT systems use different programming languages and protocols, making interoperability essential for smooth communication.  

---

##### *4. Use of different programming languages (e.g., JavaScript, Python) brings the need for interoperability.*  
- A. False  
- B. True  
*Answer:* B. True  
*Explanation:* The diversity of languages in IoT devices increases the need for interoperability so they can work together.  

---

##### *5. The interoperability between devices and users in terms of message formats is called Systematic Interoperability.*  
- A. True  
- B. False  
*Answer:* A. True  
*Explanation:* Systematic interoperability ensures devices and users understand the same message formats for communication.  

---

##### *6. What is the full form of UMB in IoT interoperability?*  
- A. Universal Meta Bridge  
- B. Universal Main Bridge  
- C. Universal Main Bracket  
- D. None of these  
*Answer:* A. Universal Meta Bridge  
*Explanation:* UMB stands for Universal Meta Bridge, helping devices with different standards connect and exchange data.  

---

##### *7. Arduino is an open-source electronic programmable board.*  
- A. True  
- B. False  
*Answer:* A. True  
*Explanation:* Arduino is widely used for building IoT projects due to its simplicity and open-source nature.  

---

##### *8. Additional circuits are essential to load a program into the Arduino controller board.*  
- A. True  
- B. False  
*Answer:* B. False  
*Explanation:* Arduino boards can be programmed directly using a USB cable, without additional circuits.  

---

##### *9. Arduino UNO has _________ number of Digital I/O pins.*  
- A. 8  
- B. 13  
- C. 14  
- D. None of these  
*Answer:* C. 14  
*Explanation:* The Arduino UNO has 14 digital input/output pins, allowing control over various components.  

---

##### *10. What does the following code do?*  
```
int ledPin = 13;
void setup() {
    pinMode(ledPin, OUTPUT);
    for (int i = 0; i < 3; i++) {
        digitalWrite(ledPin, HIGH);
        delay(1000);
        digitalWrite(ledPin, LOW);
        delay(500);
    }
}
void loop() {
    // Do nothing
}
```
- A) Blink 3 times with 1000ms ON and 500ms OFF  
- B) Blink 3 times with 500ms ON and 500ms OFF  
- C) Blink 3 times with 1000ms ON and 1000ms OFF  
- D) Stay ON continuously  
*Answer:* A) Blink 3 times with 1000ms ON and 500ms OFF  
*Explanation:* The code sets pin 13 as output, turns the LED ON for 1 second, OFF for 0.5 seconds, and repeats this 3 times.  

---

##### *11. How many types of loops are in Arduino Programming?*  
- A. 1  
- B. 2  
- C. 3  
- D. 4  
*Answer:* C. 3  
*Explanation:* Arduino supports three loops: for, while, and do-while loops.  

---

##### *12. Choose the correct syntax for the conditional (ternary) operator.*  
- A. Val = (condition)?(Statement 1):(Statement 2)  
- B. Val = (condition)?(Statement 2):(Statement 1)  
- C. Val = (condition):(Statement 1)?(Statement 2)  
- D. Val = (condition):(Statement 2)?(Statement 1)  
*Answer:* A. Val = (condition)?(Statement 1):(Statement 2)  
*Explanation:* The ternary operator returns Statement 1 if the condition is true, otherwise it returns Statement 2.  

---

##### **13. What is the purpose of calling dht.begin(); in the setup() function?**  
- A) To initialize the Serial Monitor  
- B) To start communication with the DHT sensor  
- C) To set the temperature and humidity values to zero  
- D) To define the data pin for the sensor  
*Answer:* B) To start communication with the DHT sensor  
*Explanation:* The dht.begin() function initializes the sensor so it can start reading data.  

---

##### *14. What function reads the humidity value from the DHT sensor?*  
- A) dht.getHumidity()  
- B) dht.readTemp()  
- C) dht.readHumidity()  
- D) dht.getTemperature()  
*Answer:* C) dht.readHumidity()  
*Explanation:* The readHumidity() function returns the current humidity value from the sensor.  

---

##### *15. What function sets the servo motor to a specific angle?*  
- A) ServoDemo.move()  
- B) ServoDemo.rotate()  
- C) ServoDemo.write()  
- D) ServoDemo.setAngle()  
*Answer:* C) ServoDemo.write()  
*Explanation:* The write() function sets the servo motor to a desired angle (0 to 180 degrees).  

---
