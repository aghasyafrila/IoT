# UASIoT_TID_V3920002_AghaSyafrila
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
  
 ![3](https://user-images.githubusercontent.com/89903725/146653883-c3c85721-1b4f-4bc8-ba51-22b00c099b5a.png)

Setelah tercompile ambil link file hexnya dan ketika kembali ke proteus dan program di play  led akan menyala serta muncul Virtual terminal yang memuat IP address yang digunakan untuk memuat server online/web.
  
![a](https://user-images.githubusercontent.com/89903725/143770913-15240215-5cbf-4851-929d-2f92b3d7fde8.png)

Pada bagian DNS masih 0 dan Failed to access Ethernet controller karena belum menggunakan ethernet arduino, dan IP tersebut merupakan IP atau alamat tampilan Web.
