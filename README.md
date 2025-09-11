# Whiteout Survival Bot - Interne Spielwiese

Dies ist eine interne Spielwiese zum Testen und Experimentieren mit dem Whiteout Survival Bot. Hier werden neue Features ausprobiert und getestet, bevor sie in die Hauptversion übernommen werden.

## 🧪 Experimentelle Features

Hier werden neue Bot-Funktionen getestet:

- ✅ Multi-profile support (run multiple accounts simultaneously)
- ✅ Automates daily **Nomadic Merchant** interactions
- ✅ Automatically buys **VIP points** from the merchant
- ✅ **Hero Recruitment** automation
- ✅ Collects **Daily Shards** from the **War Academy**
- ✅ Collects **Fire Crystals** from the **Crystal Laboratory**
- ✅ Opens **Exploration Chests**
- ✅ Claims **Daily VIP Points**
- ✅ Contributes to **Alliance Tech**
- ✅ Collects **Alliance Chests**
- ✅ Auto **Trains and Promotes Troops**
- ✅ Auto activates **Pet Skills** (Food, Treasure and Stamina)
- ✅ Claims **Online Rewards**
- ✅ Claims **Pet Adventure** chests
- ✅ Auto-collect rewards from mail
- ✅ **Alliance Auto Join** for rallies
- ✅ Automatically **Gathers** resources
- ✅ Automate **Intel** completion
- ✅ Claims **Tundra Trek Supplies**
- ✅ Automates **Tundra Truck Event** "My Trucks" section

## 🔧 Aktuelle Bugfixes

### Stamina OCR-Problem behoben
- **Problem:** Bot erkannte nur erste Ziffer bei Stamina-Werten über 1000 (z.B. "1" statt "1454")
- **Lösung:** Verbesserte OCR-Text-Bereinigung und erweiterte Erkennungsregion
- **Status:** ✅ Behoben - Stamina-Werte werden jetzt korrekt erkannt

### March Queue Koordination implementiert
- **Problem:** Intel und Gathering Tasks konkurrierten um die gleichen March-Slots
- **Lösung:** Intelligente Task-Koordination verhindert March-Queue-Konflikte
- **Details:** 
  - Gathering wartet wenn Intel aktiv/geplant ist (30min Fenster)
  - Intel wartet wenn Gathering aktiv/geplant ist (20min Fenster)
  - Automatische Rescheduling bei Konflikten
- **Status:** ✅ Implementiert - Optimale March-Slot-Nutzung

---

## ⚙️ Konfiguration

Der Bot ist für **MuMu Player** konfiguriert mit folgenden Einstellungen:

- **Auflösung:** 720x1280 (320 DPI)  
- **CPU:** 2 Kerne  
- **RAM:** 2GB 
- **Sprache:** Englisch

---

## 🛠️ Kompilieren & Ausführen

### Kompilieren:

```sh
mvn clean install package
```
Erstellt eine `.jar` Datei im `wos-hmi/target` Verzeichnis.

### Ausführen:

#### Über Kommandozeile (Empfohlen)
Ausführung über die Kommandozeile zeigt Echtzeit-Logs an, was beim Debugging hilfreich ist.
```sh
# In das target Verzeichnis navigieren und Bot starten
java -jar wos-bot-x.x.x.jar
```

#### Per Doppelklick
Der Bot kann auch durch Doppelklick auf die `wos-bot-x.x.x.jar` Datei gestartet werden. Dabei wird keine Konsole für Logs angezeigt.

---

### � Test-Features (In Entwicklung)
- 🔹 **Arena Kämpfe** – Automatische Arena-Verwaltung
- 🔹 **Bestien-Jagd** – Automatische Bestien-Jagd implementieren
- 🔹 **Polar Terror Jagd** – Automatische Polar Terror Jagd implementieren
- 🔹 **Und mehr...** 🔥




