# Netzwerk

Diese Datei enthält wichtige Linux-Befehle für die Netzwerkverwaltung und Fehleranalyse.

## ping

Prüft, ob ein anderer Rechner oder eine Website erreichbar ist.

Beispiele:

```bash
ping google.com
ping 8.8.8.8
ip

Zeigt Informationen zu Netzwerkschnittstellen und IP-Adressen an.

Beispiele:

ip a
ip addr
ip route
hostname

Zeigt den Rechnernamen an.

hostname
nslookup

Fragt DNS-Informationen zu einer Domain ab.

nslookup google.com
nslookup openai.com
traceroute

Zeigt den Weg der Datenpakete bis zum Ziel.

traceroute google.com
ss

Zeigt aktive Netzwerkverbindungen an.

ss -t
ss -tuln
netstat

Zeigt Netzwerkverbindungen und offene Ports an.

netstat -tuln
curl

Ruft Daten von Webseiten oder APIs ab.

curl google.com
curl https://api.github.com
wget

Lädt Dateien aus dem Internet herunter.

wget https://example.com/datei.zip
ssh

Verbindet sich mit einem entfernten Rechner.

ssh benutzer@server
scp

Kopiert Dateien über das Netzwerk.

scp datei.txt benutzer@server:/home/benutzer
scp benutzer@server:/home/test.txt .
dig

Zeigt detaillierte DNS-Informationen an.

dig google.com
dig openai.com
Netzwerk-Konfiguration anzeigen
ip a
ip route
hostname
DNS testen
nslookup google.com
dig google.com
Verbindung testen
ping google.com
traceroute google.com
