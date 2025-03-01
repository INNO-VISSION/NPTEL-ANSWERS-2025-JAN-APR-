# **Week 7: Internet Of Things**

#### **1. In Python socket programming, while defining a socket, SOCK_STREAM refers to a type of:**  
- A. SocketFamily  
- **B. SocketType**  
- C. SocketName  
- D. SocketProtocol  
**Answer:** B. SocketType  
**Explanation:** `SOCK_STREAM` is used to create TCP sockets, which provide reliable, connection-oriented communication.

---

#### **2. If you want to change the label of the Y-axis while plotting a graph using matplotlib in Python, what among the following functions do you use? Suppose you have imported matplotlib as plt**  
- A. plt.show()  
- B. plt.plot()  
- **C. plt.ylabel()**  
- D. plt.yaxis()  
**Answer:** C. plt.ylabel()  
**Explanation:** The `plt.ylabel()` function sets the label for the Y-axis in a plot.

---

#### **3. In socket programming, AF_INET stands for:**  
- A. Unix protocols  
- **B. Internet Protocol (IP)**  
- C. File sharing  
- D. Time slicing  
**Answer:** B. Internet Protocol (IP)  
**Explanation:** `AF_INET` refers to the IPv4 address family for sockets.

---

#### **4. Suppose a Python server is receiving data from a socket as follows,**  
```python
data, addr = sock.recvfrom(1024)
```  
**What kind of socket is used in this code?**
- A. TCP socket  
- **B. UDP socket**  
- C. TAP socket  
- D. None of the given  
**Answer:** B. UDP socket  
**Explanation:** `recvfrom()` is used with UDP sockets, which are connectionless.

---

#### **5. What is the use of the Mobi-Flow protocol?**  
- A. Enabling static SDN  
- **B. Enabling SDN to incorporate mobility**  
- C. Enabling Odin Master  
- D. Enabling traditional BGP  
**Answer:** B. Enabling SDN to incorporate mobility  
**Explanation:** Mobi-Flow extends SDN to handle mobile devices and dynamic topology changes.

---

#### **6. During remote server access using socket programming what is the utility of the .<socket_name>.listen() function?**  
- A. To create a new socket  
- B. To bind the socket to a connection  
- **C. To wait for clients to connect**  
- D. To close the connection  
**Answer:** C. To wait for clients to connect  
**Explanation:** `listen()` makes the socket listen for incoming client connections.

---

#### **7. Which among the following is the correct direction for PACKET_OUT type messages in SDN?**  
- **A. From controller to switch**  
- B. From switch to controller  
- C. Between two switches  
- D. Between two controllers  
**Answer:** A. From controller to switch  
**Explanation:** `PACKET_OUT` messages are sent from the SDN controller to switches to push flow entries or packets.

---

#### **8. Which among the following is a limitation of the traditional non-SDN networks?**  
- A. Switches do not possess a routing table  
- B. Switches are unable to forward traffic  
- **C. Switches do not have a global view of the network**  
- D. All of the given  
**Answer:** C. Switches do not have a global view of the network  
**Explanation:** Traditional switches lack centralized control, limiting their network-wide awareness.

---

#### **9. During remote server access by a Raspberry Pi, where the Raspberry Pi acts as a client, the client needs the following?**  
- A. Only IP address of server  
- B. Only port number  
- **C. Both server IP address and port number**  
- D. Client’s IP address  
**Answer:** C. Both server IP address and port number  
**Explanation:** The IP identifies the server, while the port specifies the service.

---

#### **10. With respect to the concept of soft time-out and hard time-out in SDN switches, which of the following relations hold?**  
- A. Soft time-out >= hard time-out  
- **B. Hard time-out >= soft time-out**  
- C. Soft time-out = hard time-out always  
- D. None of the given  
**Answer:** B. Hard time-out >= soft time-out  
**Explanation:** A flow rule expires after a hard time-out, even if packets are still flowing (unlike a soft time-out).

---

#### **11. Which of the following is true?**  
- A. Traditional Network: Routing Table, SDN: Routing Table  
- B. Traditional Network: Flow Table, SDN: Routing Table  
- **C. Traditional Network: Routing Table, SDN: Flow Table**  
- D. Traditional Network: Flow Table, SDN: Flow Table  
**Answer:** C. Traditional Network: Routing Table, SDN: Flow Table  
**Explanation:** Traditional networks use routing tables, while SDN uses flow tables to handle traffic.

---

#### **12. Consider the following figure below. To which issue of SDN does this particular figure can be related to?**  
- **A. Controller placement issue**  
- B. Flow Rule placement issue  
- C. Hardware placement issue  
- D. Analysis placement issue  
**Answer:** A. Controller placement issue  
**Explanation:** Proper controller placement affects SDN performance and fault tolerance.

---

#### **13. With respect to the directional APIs in SDN, what is the functionality of East-Westbound APIs?**  
- A. To communicate between the controller and switches  
- **B. To communicate among multiple controllers**  
- C. East-Westbound APIs do not exist  
- D. To communicate between switches themselves  
**Answer:** B. To communicate among multiple controllers  
**Explanation:** East-Westbound APIs allow communication and state sharing between SDN controllers.

---

#### **14. Hierarchical SDN architecture is also known as:**  

- **A. Tree**  
- B. Flat  
- C. Mesh  
- D. Line  
**Answer:** A. Tree  
**Explanation:** Hierarchical SDN uses a tree-like structure to manage different control planes.

---

#### **15. Integrating SDN with IoT is not recommended and is not a suitable approach to follow**  
- **A. False**  
- B. True  
**Answer:** A. False  
**Explanation:** SDN enhances IoT by providing centralized control, dynamic routing, and better scalability.

---
