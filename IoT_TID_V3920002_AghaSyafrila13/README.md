# IoT_TID_V3920002_AghaSyafrila
Komunikasi Ethernet menggunakan Proteus dan Arduino.
Rangkaian menggunakan Arduino Uno R3, Modul Ethernet ENC28J60, Virtual Terminal, 4 LED, LM35 (data konverter), MCP 9701A

Sebelum mengcompile script harus ditambahkan library untuk ethernet melalui sketch kemudian include library. Kemudian ubah **#define STATIC 0  // set to 1 to disable DHCP (adjust myip/gwip values below)** menjadi **#define STATIC 1  // set to 1 to disable DHCP (adjust myip/gwip values below)** dan 
  void setup(){
  Serial.begin **(57600);**
  Serial.println("\n[backSoon]"); 
  
  menjadi 
  
  void setup(){
  Serial.begin **(9600);**
  Serial.println("\n[backSoon]");. 
  
  **(bagian program yang memuat tampilan web)**
  
  ![scr](https://user-images.githubusercontent.com/89903725/143771752-1440c044-6486-4a9a-ad8b-32d8eda5746f.png)

Setelah tercompile ambil link file hexnya dan ketika kembali ke proteus dan program di play  led akan menyala serta muncul Virtual terminal yang memuat IP address yang digunakan untuk memuat server online/web.
  
![a](https://user-images.githubusercontent.com/89903725/143770913-15240215-5cbf-4851-929d-2f92b3d7fde8.png)

Pada bagian DNS masih 0 dan Failed to access Ethernet controller karena belum menggunakan ethernet arduino.

![b](https://user-images.githubusercontent.com/89903725/143771092-cf2687ae-d03c-49b1-95f4-338abaf5d4ff.png)
  
