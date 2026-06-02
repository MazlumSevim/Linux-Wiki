# Bash-Skripte

Diese Datei erklärt die Grundlagen von Bash-Skripten unter Linux.

## Was ist ein Bash-Skript?

Ein Bash-Skript ist eine Textdatei mit mehreren Linux-Befehlen, die automatisch nacheinander ausgeführt werden.

Beispiel:

```bash
#!/bin/bash

echo "Hallo Welt"
Skript erstellen

Datei erstellen:

touch skript.sh

Datei bearbeiten:

nano skript.sh
Skript ausführbar machen
chmod +x skript.sh
Skript ausführen
./skript.sh

oder

bash skript.sh
Variablen

Variablen speichern Werte.

#!/bin/bash

name="Max"
echo $name

Ausgabe:

Max
Benutzereingaben
#!/bin/bash

read name
echo "Hallo $name"
if-Abfrage
#!/bin/bash

zahl=10

if [ $zahl -gt 5 ]
then
    echo "Zahl ist größer als 5"
fi
if-else
#!/bin/bash

zahl=3

if [ $zahl -gt 5 ]
then
    echo "Größer als 5"
else
    echo "Kleiner oder gleich 5"
fi
for-Schleife
#!/bin/bash

for i in 1 2 3 4 5
do
    echo $i
done
while-Schleife
#!/bin/bash

x=1

while [ $x -le 5 ]
do
    echo $x
    x=$((x+1))
done
Funktionen
#!/bin/bash

hallo() {
    echo "Hallo Welt"
}

hallo
Dateien prüfen
#!/bin/bash

if [ -f datei.txt ]
then
    echo "Datei vorhanden"
fi
Verzeichnisse prüfen
#!/bin/bash

if [ -d ordner ]
then
    echo "Ordner vorhanden"
fi
Kommentare
# Das ist ein Kommentar
echo "Hallo"
Nützliche Befehle in Skripten
date
pwd
whoami
hostname
Beispielskript
#!/bin/bash

echo "Systeminformationen"

echo "Benutzer:"
whoami

echo "Verzeichnis:"
pwd

echo "Datum:"
date
