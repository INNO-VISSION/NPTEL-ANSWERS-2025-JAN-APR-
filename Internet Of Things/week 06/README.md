#### *Week 6:  Introduction To Internet Of Things*  

##### *1. Python is popular for embedded application development as it is a very lightweight programming language.*  
- A. True  
- B. False  
*Answer:* A. True  
*Explanation:* Python is widely used for embedded systems and IoT projects because of its simplicity and lightweight nature.  

---

##### *2. Adafruit provides a library to work with DHT22 Sensor.*  
- A. True  
- B. False  
*Answer:* A. True  
*Explanation:* Adafruit offers libraries like Adafruit_DHT to interact with DHT22 sensors for temperature and humidity readings.  

---

##### *3. What is the output of the following Python code?*  
```
x = [4, 5, 6]
y = [str(x[0] + 1), str(len(x) * 2) + '&Code']
z = y[1].split('&')
print(z[1])
```
- A. 5  
- B. 12  
- C. Code  
- D. &Code  
*Answer:* C. Code  
*Explanation:* The split() function splits the string "12&Code" at &, so z becomes ['12', 'Code'], and z[1] prints "Code".  

---

##### *4. Python follows rigid indentation to indicate different blocks of code.*  
- A. True  
- B. False  
*Answer:* A. True  
*Explanation:* Python uses indentation to define code blocks, and incorrect indentation will raise an error.  

---

##### *5. What is the output of this code?*  
python
print "Hi, Welcome to python!"

- A. Hi, Welcome to python!  
- B. “Hi, Welcome to python!”  
- C. Hi, Welcome to python  
- D. None of these  
*Answer:* D. None of these  
*Explanation:* In Python 3, print needs parentheses. The above code works only in Python 2, so in Python 3, it throws a syntax error.  

---

##### *6. During remote server access by a Raspberry Pi, the client needs:*  
- A. Only IP address of server  
- B. Only port number  
- C. Both server IP address and port number  
- D. Client’s IP address  
*Answer:* C. Both server IP address and port number  
*Explanation:* The IP address identifies the server, and the port number specifies the service to connect to.  

---

##### *7. Is this command correct to install the PIL library?*  
bash
sudo pip install pillow

- A. Correct  
- B. Incorrect  
*Answer:* A. Correct  
*Explanation:* Pillow is the modern version of the PIL library, and this command correctly installs it.  

---

##### **8. What is the purpose of the "w" mode in the open() function?**  
- A) To read a file  
- B) To write data to a file, overwriting existing content  
- C) To append data to a file  
- D) To open a file in read and write mode  
*Answer:* B) To write data to a file, overwriting existing content  
*Explanation:* The "w" mode opens a file for writing, creating a new file or overwriting existing content.  

---

##### *9. What will be the output of this code?*  
python
with open("PythonProgram.txt", "w") as file:
    file.write("Writing data")
with open("PythonProgram.txt", "r") as file:
    f = file.read()
    print('Reading from the file\n')
    print(f)

- A) Writing data  
- B) Reading from the file Writing data  
- C) Error: File not found  
- D) None of the above  
*Answer:* B) Reading from the file Writing data  
*Explanation:* The code writes "Writing data" to the file, then reads and prints the content.  

---

##### *10. Can we configure Raspberry Pi as a File Server?*  
- A. Yes  
- B. No  
*Answer:* A. Yes  
*Explanation:* Raspberry Pi can be configured as a file server using tools like Samba or NFS.  

---

##### *11. Which command configures the Raspberry Pi for the camera module?*  
- A) sudo camera-config  
- B) sudo raspi-config  
- C) sudo enable-camera  
- D) sudo pi-setup  
*Answer:* B) sudo raspi-config  
*Explanation:* The raspi-config tool is used to enable and configure hardware like the camera module.  

---

##### *12. What is the final step after enabling the camera?*  
- A) Restart the camera service  
- B) Run a camera test command  
- C) Reboot the Raspberry Pi  
- D) Reinstall the Raspberry Pi OS  
*Answer:* C) Reboot the Raspberry Pi  
*Explanation:* After enabling the camera, a reboot is necessary for the changes to take effect.  

---

##### *13. Which command exits the Nano editor?*  
- A. Ctrl + X  
- B. Ctrl + O  
- C. Ctrl + K  
- D. None of these  
*Answer:* A. Ctrl + X  
*Explanation:* Ctrl + X exits the Nano editor, and you can choose to save changes.  

---

##### *14. When should the fan turn on in a temperature-controlled system?*  
- A) When the relay is manually triggered  
- B) When the surrounding temperature is lower than a predefined threshold  
- C) When the surrounding temperature exceeds a predefined threshold  
- D) When the battery voltage drops below a certain level  
*Answer:* C) When the surrounding temperature exceeds a predefined threshold  
*Explanation:* The relay turns on the fan when the temperature surpasses a set value, cooling the system.  

---

##### *15. What does this command do?*  

- A. Captures video feed  
- B. Captures still image  
- C. Both (a) and (b)  
- D. None of these  
*Answer:* B. Captures still image  
*Explanation:* The raspistill command captures a still image and saves it as image.jpg.  

---
