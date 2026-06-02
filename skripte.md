# 📜 Bash-Skripte

Diese Datei erklärt die Grundlagen von Bash-Skripten unter Linux.

## 🤔 Was ist ein Bash-Skript?

Ein Bash-Skript ist eine Textdatei mit mehreren Linux-Befehlen, die automatisch nacheinander ausgeführt werden.

Beispiel:

```bash
#!/bin/bash

echo "Hallo Welt"
```

## 📄 Skript erstellen

### `touch`

```bash
touch skript.sh    # erstellt eine neue Skriptdatei
```

### `nano`

```bash
nano skript.sh     # öffnet die Datei im Editor nano
```

## 🔐 Skript ausführbar machen

### `chmod`

```bash
chmod +x skript.sh    # macht das Skript ausführbar
```

## ▶️ Skript ausführen

```bash
./skript.sh           # führt das Skript aus
```

oder

```bash
bash skript.sh        # startet das Skript mit Bash
```

## 📦 Variablen

Variablen speichern Werte.

```bash
#!/bin/bash

name="Max"            # Variable erstellen

echo $name            # Variable ausgeben
```

## ⌨️ Benutzereingaben

Mit `read` können Eingaben gespeichert werden.

```bash
#!/bin/bash

read name             # Eingabe speichern

echo "Hallo $name"
```

## ❓ if-Abfrage

Führt Befehle nur aus, wenn eine Bedingung erfüllt ist.

```bash
#!/bin/bash

zahl=10

if [ $zahl -gt 5 ]
then
    echo "Zahl ist größer als 5"
fi
```

## 🔀 if-else

```bash
#!/bin/bash

zahl=3

if [ $zahl -gt 5 ]
then
    echo "Größer als 5"
else
    echo "Kleiner oder gleich 5"
fi
```

## 🔁 for-Schleife

Wiederholt Befehle mehrmals.

```bash
#!/bin/bash

for i in 1 2 3 4 5
do
    echo $i
done
```

## 🔄 while-Schleife

Wiederholt Befehle solange eine Bedingung erfüllt ist.

```bash
#!/bin/bash

x=1

while [ $x -le 5 ]
do
    echo $x
    x=$((x+1))
done
```

## 🛠️ Funktionen

Funktionen fassen Befehle zusammen.

```bash
#!/bin/bash

hallo() {
    echo "Hallo Welt"
}

hallo
```

## 📂 Prüfen, ob eine Datei existiert

```bash
#!/bin/bash

if [ -f datei.txt ]
then
    echo "Datei vorhanden"
fi
```

## 📁 Prüfen, ob ein Ordner existiert

```bash
#!/bin/bash

if [ -d ordner ]
then
    echo "Ordner vorhanden"
fi
```

## 💬 Kommentare

Kommentare werden nicht ausgeführt und dienen zur Erklärung.

```bash
# Das ist ein Kommentar

echo "Hallo"
```

## 🖥️ Nützliche Befehle in Skripten

```bash
date       # aktuelles Datum anzeigen
pwd        # aktuelles Verzeichnis anzeigen
whoami     # aktuellen Benutzer anzeigen
hostname   # Rechnernamen anzeigen
```

## 🚀 Beispielskript

```bash
#!/bin/bash

echo "Systeminformationen"

echo "Benutzer:"
whoami

echo "Verzeichnis:"
pwd

echo "Datum:"
date
```

## 📋 Zusammenfassung

```bash
touch skript.sh      # Skript erstellen
nano skript.sh       # Skript bearbeiten
chmod +x skript.sh   # ausführbar machen
./skript.sh          # Skript starten
```
