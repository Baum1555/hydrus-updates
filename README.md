# HYDRUS-Updates

Version **2.1.6** für Heltec WiFi LoRa 32 V3 (ESP32-S3/SX1262) und das lokale Windows-Programm.

- [Komplettpaket mit Arduino-Quellcode und PC-Programm](releases/Hydrus-2.1.6.zip)
- [Signiertes Heltec-Update](releases/heltec-2.1.6.hup)
- [Signiertes PC-Update](releases/pc-2.1.6.hup)

Neu in 2.1.6: sichtbare Batterierestlaufzeit, Temperaturen, Zählerstatus und weitere übertragene Werte. Warnregeln mit verständlichen Bezeichnungen und Live-Zusammenfassung. Das in der Weboberfläche gespeicherte Accesspoint-Passwort bleibt bei Online-Updates erhalten.

Die Oberfläche zeigt Ladeanimationen bei der Updatesuche und Heltec-Onlineinstallation, Prozentwerte bei PC-Downloads und Firmware-Uploads sowie den Abschlussstatus.

Ein mitgeliefertes Zertifikatspaket unterstützt beide HTTPS-Schnittstellenvarianten, auch die des Heltec-Pakets 3.0.3.

Enthalten: gespeicherte Warnereignisse, geführter Messmengenvergleich, optionale ntfy-Mitteilungen und vorbereitete Online-Updates. Die gesamte Weboberfläche ist ohne zusätzliche Admin-Anmeldung bedienbar.

Version 2.1 kann über die lokale Datei-Auswahl im Update-Tab einer passenden 2.0-Installation eingespielt werden. Alternativ Arduino-Quellcode über USB hochladen. Zählerkonfiguration und Heimnetzzugang im NVS bleiben bei unveränderter Partitionierung erhalten. Ohne gespeichertes Accesspoint-Passwort gilt `Hydrus-Lokal-2026`. Ein ab 2.1.5 über die Einstellungen gespeichertes Passwort bleibt bei Updates erhalten. Neue Geräte benötigen ihre eigenen Zählerkennungen und Schlüssel in den Einstellungen.

Die Firmware wurde gebaut und simuliert getestet. Echter Funkbetrieb, OTA auf Hardware und Push-Zustellung müssen am Gerät geprüft werden. Leckverdacht ist kein garantierter Lecknachweis. Der Messvergleich verändert keine Messwerte.

## Versionsadressen

Heltec: `https://raw.githubusercontent.com/Baum1555/hydrus-updates/main/heltec-version.json`

PC: `https://raw.githubusercontent.com/Baum1555/hydrus-updates/main/pc-version.json`

Ab Version 2.1 sind diese Adressen voreingestellt. Updates werden signiert und erst nach Bestätigung installiert. Das CA-Feld kann bei GitHub ab Version 2.1 leer bleiben. Der private Signaturschlüssel bleibt beim Herausgeber; dieses Repository enthält weder ihn noch persönliche AES-Zählerschlüssel.
