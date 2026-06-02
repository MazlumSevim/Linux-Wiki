# 🌐 Netzwerk

Diese Datei enthält wichtige Linux-Befehle für Netzwerkverwaltung und Fehleranalyse.

## 📡 Verbindung testen

### `ping`

Prüft, ob ein anderer Rechner oder eine Webseite erreichbar ist.

```bash
ping google.com    # testet die Verbindung zu Google
ping 8.8.8.8       # testet die Verbindung zu einer IP-Adresse
```

## 🖥️ IP-Adresse anzeigen

### `ip`

Zeigt Netzwerkinformationen an.

```bash
ip a         # zeigt alle Netzwerkschnittstellen und IP-Adressen
ip addr      # gleiche Funktion wie ip a
ip route     # zeigt die Routing-Tabelle an
```

## 🏷️ Rechnernamen anzeigen

### `hostname`

```bash
hostname     # zeigt den Namen des Computers an
```

## 🔍 DNS-Abfrage

### `nslookup`

Fragt Informationen über eine Domain ab.

```bash
nslookup google.com   # zeigt DNS-Informationen von Google
nslookup openai.com   # zeigt DNS-Informationen von OpenAI
```

## 🛣️ Verbindungsweg anzeigen

### `traceroute`

Zeigt den Weg der Datenpakete bis zum Ziel.

```bash
traceroute google.com   # zeigt die einzelnen Stationen bis Google
```

## 🔌 Netzwerkverbindungen anzeigen

### `ss`

Zeigt aktive Netzwerkverbindungen an.

```bash
ss -t      # zeigt TCP-Verbindungen
ss -tuln   # zeigt offene Ports und Verbindungen
```

## 📊 Netzwerkstatistik anzeigen

### `netstat`

```bash
netstat -tuln   # zeigt offene Ports und aktive Verbindungen
```

## 🌍 Webseiten abrufen

### `curl`

Ruft Daten von Webseiten oder APIs ab.

```bash
curl google.com              # lädt den Quelltext der Webseite
curl https://api.github.com  # ruft Daten einer API ab
```

## ⬇️ Dateien herunterladen

### `wget`

```bash
wget https://example.com/datei.zip   # lädt eine Datei herunter
```

## 🔐 Verbindung zu einem Server

### `ssh`

Verbindet sich mit einem entfernten Rechner.

```bash
ssh benutzer@server   # verbindet sich mit einem Server
```

## 📂 Dateien über Netzwerk kopieren

### `scp`

```bash
scp datei.txt benutzer@server:/home/benutzer   # Datei auf Server kopieren
scp benutzer@server:/home/test.txt .           # Datei vom Server herunterladen
```

## 📋 Zusammenfassung

```bash
ping google.com       # Verbindung testen
ip a                  # IP-Adresse anzeigen
hostname              # Rechnername anzeigen
nslookup google.com   # DNS-Abfrage
ssh benutzer@server   # Serververbindung
```
