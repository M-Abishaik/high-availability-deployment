# Steps
1. Download code-deployment.ino in the Node-MCU & add WIFI SSIDs in KNOWN_SSID[] and the password of WIFI SSIDs in KNOWN_PASSWORD[].
2. Flash the file in the ESP-8266 Node MCU board and after the wifi scan, the NodeMCU client will connect to the Primary SSID.
3. To simulate failover, intentionally flap the port/power-off the switch and ensure that the primary SSID goes down.
4. After the AP is down, the Node-MCU client will connect to its backup AP in the least amount of time providing almost zero down-time.
5. The new system can be reverted to the original state either automatically follwing the same procedure or manually via a network admin. 


