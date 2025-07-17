# PoolButtler
Der PoolButtler kümmerst sich wie ein Poolboy um deinen Pool. Er misst und speichert die Daten deines Swimming Pools.

💡 Funktionen der Überwachungsstation

1. Chlorgehalt messen (freies Chlor)
2. pH-Wert erfassen
3. Wasserqualität bestimmen (z. B. Leitfähigkeit, Trübung, Temperatur)

🔧 Benötigte Hardware (Vorschlag)

| Komponente | Beschreibung |
|------------|--------------|
| Microcontroller | ESP32 oder Arduino Uno/Mega |
| pH-Sensor | Analog pH-Sensor Modul (z. B. von DFRobot) |
| Chlor-Sensor | Spezielle galvanische oder amperometrische Sensoren für freies Chlor (z. B. von Atlas Scientific oder SEN0161) |
| Temperatursensor | DS18B20 (wasserdicht) |
| Trübungssensor | SEN0189 (DFRobot) |
| EC-Sensor | Für Leitfähigkeit (Gesamtwasserqualität) |
| Display | OLED oder LCD zur Anzeige vor Ort |
| WLAN-Modul | Im ESP32 enthalten, falls Fernüberwachung gewünscht ist |

⚙️ Software

- Messung der Sensorwerte in regelmäßigen Abständen
- Speicherung auf SD-Karte oder Übertragung via WLAN (z. B. an eine App oder Webserver)
- Alarme bei Grenzwertüberschreitung
- Kalibrierung der Sensoren

📱 Erweiterungen

- Web-Interface (ESP32 als Webserver)
- Benachrichtigung per E-Mail/Push
- Integration in Home Assistant