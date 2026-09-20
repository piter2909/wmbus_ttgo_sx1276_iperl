## Sensus (iPerl), LoRa 868 MHz, Radio water meter receiver for TTGO SX1276


Data is send via MQTT, Home Assistant will automatically discover entities

## Board:
<img width="194" height="340" alt="image" src="https://github.com/user-attachments/assets/8898b365-ee0f-4634-87b1-3b595af5ba97" />
<img width="398" height="362" alt="image" src="https://github.com/user-attachments/assets/e12c9963-f2d9-4a1d-bcf9-732fd7f621ef" />


<img width="572" height="407" alt="image" src="https://github.com/user-attachments/assets/5fe90c07-48be-4622-8755-8b432dc73bca" />

## Arduino IDE Settings:
```bash
  Board: ESP32 Dev Module
  Partition scheme: Default 4MB with spiffs
  PSRAM: Disabled
```
External library required: PubSubClient (Nick O'Leary)

## Default configuration values to edit.
```javascript
// --- WiFi ---
WIFI_SSID = "TwojeSSID";
WIFI_PASS = "TwojeHaslo";

// --- MQTT ---
MQTT_HOST = "192.168.1.10";
MQTT_PORT = 1883;
MQTT_USER = "mqtt_user";
MQTT_PASS = "mqtt_pass";

// --- Device name ---
NODE_ID   = "wmbus_water";                          // unique device ID
NODE_NAME = "Wodomierz wM-Bus";                     // Home Assistant name

// --- Licznik ---
METER_ID = "12345678";

// --- AES-128 Key ---
METER_KEY_HEX = "00112233445566778899AABBCCDDEEFF";

// ---  NTP Server---
NTP_SERVER = "pl.pool.ntp.org";
```

## Home Assistant entities:


<img width="321" height="503" alt="wmbus" src="https://github.com/user-attachments/assets/a25a907f-a58b-4611-afab-1b3582522f6a" />


Made by AI
