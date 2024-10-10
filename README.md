# ![Icon](https://raw.githubusercontent.com/mathoudebine/turing-smart-screen-python/main/res/icons/monitor-icon-17865/24.png) turing-smart-screen-python

### ⚠️ HAFTUNGSAUSSCHLUSS - BITTE LESEN ⚠️

Dieses Projekt ist **weder mit den Marken Turing / XuanFang / Kipye noch mit deren Tochtergesellschaften, Partnern, Herstellern oder Verkäufern ihrer Produkte verbunden, assoziiert, autorisiert oder in irgendeiner Weise offiziell verknüpft**. Alle Produkt- und Firmennamen sind eingetragene Marken ihrer ursprünglichen Eigentümer.

Dieses Projekt ist eine Open-Source-Softwarealternative, NICHT die Originalsoftware für die Smart-Bildschirme. **Bitte keine Probleme bezüglich USBMonitor.exe/ExtendScreen.exe oder der Hardware der Smart-Bildschirme hier melden**.
* Für den Turing Smart Screen, nutze das offizielle Forum hier: http://discuz.turzx.com/
* Für andere Smart-Bildschirme, kontaktiere deinen Händler
---

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white) ![macOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=Raspberry%20Pi&logoColor=white) ![Python](https://img.shields.io/badge/Python-3.8/3.12-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) [![Lizenz](https://img.shields.io/github/license/mathoudebine/turing-smart-screen-python?style=for-the-badge)](./LICENSE)
  

Ein Python-Systemüberwachungsprogramm und eine Abstraktionsbibliothek für **kleine IPS USB-C (UART) Displays.**    

Unterstützte Betriebssysteme: macOS, Windows, Linux (inkl. Raspberry Pi), im Grunde alle Betriebssysteme, die Python 3.8+ unterstützen  

### Unterstützte Smart-Bildschirm-Modelle:

| ✅ Turing Smart Screen 3.5"                           | ✅ XuanFang 3.5"                                   | ✅ Turing Smart Screen 5"                    |
|------------------------------------------------------|---------------------------------------------------|---------------------------------------------|
| <img src="res/docs/turing.webp"/>                    | <img src="res/docs/xuanfang.webp"/>               | <img src="res/docs/turing5inch.png"/>       |
| Auch fälschlicherweise von den Händlern "Revision A" genannt | Revision B & Flaggschiff (mit Rückplatte & RGB-LEDs) | Grundlegende Unterstützung (kein Video oder Speicher vorerst) |

| ✅ [UsbPCMonitor 3.5" / 5"](https://aliexpress.com/item/1005003931363455.html)                       | ✅ [Kipye Qiye Smart Display 3.5"](https://www.aliexpress.us/item/3256803899049957.html) |
|-----------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|
| <img src="res/docs/UsbPCMonitor_5inch.webp" width="60%" height="60%"/>                              | <img src="res/docs/kipye-qiye-35.webp" width="60%" height="60%"/>                       |
| Unbekannter Hersteller, optisch ähnlich zum Turing 3.5" / 5". Originalsoftware ist `UsbPCMonitor.exe` | Frontplatte hat eine eingravierte Aufschrift "奇叶智显" Qiye Zhixian (Qiye Smart Display)        |

### [> Welches Smart-Bildschirm-Modell habe ich?](https://github.com/mathoudebine/turing-smart-screen-python/wiki/Hardware-revisions)  

**Bitte beachte, dass alle aufgeführten Smart-Bildschirme unterschiedliche Produkte** sind, die von verschiedenen Unternehmen entworfen und produziert wurden, obwohl sie ein ähnliches Erscheinungsbild haben. Auch ihr Kommunikationsprotokoll ist unterschiedlich.  
Dieses Projekt bietet eine Abstraktionsschicht, um all diese Produkte auf einheitliche Weise zu verwalten, einschließlich einiger produktspezifischer Funktionen wie Rückplatten-RGB-LEDs für verfügbare Modelle!

Wenn du deinen Bildschirm noch nicht erhalten hast, aber jetzt schon mit der Entwicklung deines Themas beginnen möchtest, kannst du den [**"simulierten LCD"-Modus!**](https://github.com/mathoudebine/turing-smart-screen-python/wiki/Simulated-display) verwenden.

### Noch nicht unterstützte / nicht getestete Smart-Bildschirm-Modelle:

| ❔ _Turing Smart Screen 8.8"_                                                                                                                     | ❔ _Turing Smart Screen 2.1"_                                                                                                                     | ❌ _[(Fuldho?) 3.5" IPS Bildschirm](https://aliexpress.com/item/1005005632018367.html)_                                                                                                                                                                                                                |
|--------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="res/docs/turing8inch.jpg"/>                                                                                                            | <img src="res/docs/turing2inch.webp"/>                                                                                                           | <img src="res/docs/fuldho_3.5.jpg"/>                                                                                                                                                                                                                                                              |
| Sehr ähnliches Protokoll wie das des 5". [Unterstützung in einer zukünftigen Version geplant.](https://github.com/mathoudebine/turing-smart-screen-python/issues/264) | Sehr ähnliches Protokoll wie das des 5". [Unterstützung in einer zukünftigen Version geplant.](https://github.com/mathoudebine/turing-smart-screen-python/issues/264) | Wird von [proprietärer Windows-Software `SmartMonitor.exe`](https://smartdisplay.lanzouo.com/b04jvavkb) verwaltet. Kann in diesem Projekt nicht unterstützt werden: [siehe hier](https://github.com/mathoudebine/turing-smart-screen-python/discussions/298). Alternative Bibliothek verwenden https://github.com/braewoods/hidss |

| ❌ _Waveshare [2.1inch](https://www.waveshare.com/wiki/2.1inch-USB-Monitor) / [2.8inch](https://www.waveshare.com/wiki/2.8inch-USB-Monitor) / [5inch](https://www.waveshare.com/wiki/5inch-USB-Monitor) / [7inch](https://www.waveshare.com/wiki/7inch-USB-Monitor) USB-Monitor_                                                                                                            | ❌ _[GUITION Smart screen](https://aliexpress.com/item/1005006169962183.html)_                                                                                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="res/docs/waveshare-21inch-28inch.png"/>                                                                                                                                                                                                                                                                                                                                          | <img src="res/docs/guition.webp"/>                                                                                                                                                                                                                                                          |
| Verkauft im [Waveshare-Shop](https://www.waveshare.com/2.8inch-usb-monitor.htm) oder [Aliexpress](https://fr.aliexpress.com/item/1005006071685067.html). Verwaltet durch [proprietäre Windows-Software "Waveshare PC Monitor"](https://github.com/mathoudebine/turing-smart-screen-python/wiki/Vendor-apps#waveshare-pc-monitor---vendor-app). Kann in diesem Projekt nicht unterstützt werden: benötigt eine Firmware. | Verwaltet durch [proprietäre Windows-Software "GUITION Smart screen"](https://github.com/mathoudebine/turing-smart-screen-python/wiki/Vendor-apps#guition---vendor-app). Kann in diesem Projekt nicht unterstützt werden: [siehe hier](https://github.com/mathoudebine/turing-smart-screen-python/issues/426). |

| ❔ _[SmartCool Lcd](https://aliexpress.com/item/1005005443609423.html) / [GeekTeches AD35](https://aliexpress.com/item/1005004858688084.html) / AIDA64 / AX206_                                   |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <img src="res/docs/ax206.jpg" width="30%" height="30%" /> <img src="res/docs/geekteches_ad35.jpg" width="30%" height="30%" /> <img src="res/docs/smartcool_lcd.webp" width="30%" height="30%" /> |
| Nicht unterstützt. Von mehreren Herstellern produziert, alle nutzen die gleiche [Appotech AX206 gehackte Bilderrahmen-Firmware](https://github.com/dreamlayers/dpf-ax). Unterstützt von AIDA64 und lcd4linux       |

## So startest du

### [> Folge den Anweisungen im Wiki, um dieses Projekt zu konfigurieren und zu starten.](https://github.com/mathoudebine/turing-smart-screen-python/wiki)

Es gibt zwei mögliche Nutzungsarten des Python-Codes dieses Projekts:
* **[als Systemmonitor](#system-monitor)**, ein eigenständiges Programm, das mit Themes arbeitet, um die Hardware-Informationen deines Computers und benutzerdefinierte Daten auf elegante Weise anzuzeigen.
[Überprüfe, ob deine Hardware unterstützt wird.](https://github.com/mathoudebine/turing-smart-screen-python/wiki/System-monitor-:-hardware-support)
* **[in dein Projekt integriert](#control-the-display-from-your-python-projects)**, um den Bildschirm vollständig aus deinem eigenen Python-Code zu steuern.

## Systemmonitor



`main.py` ist das Skript, das du ausführen solltest, um deine Computer-Statistiken auf einem Turing Smart Screen anzuzeigen.

### Voraussetzungen
Python 3.8 bis 3.12.

#### Wichtige Bibliotheken

```bash
pip install pyserial psutil pillow websockets
```

#### Starte das Programm

Um den Bildschirm zu verwenden, überprüfe, dass er in den UART-Modus (seriell) geschaltet ist.  
Die Baudrate des UART-Ports des Turing-Smart-Bildschirms muss auf 115200 eingestellt werden.

```bash
python main.py
```
