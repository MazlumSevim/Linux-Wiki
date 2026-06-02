# 💻 Linux-Befehle

Diese Datei enthält wichtige Linux-Befehle für die tägliche Arbeit im Terminal.

## 📂 Verzeichnisse anzeigen

### `ls`

Zeigt Dateien und Ordner an.

```bash
ls          # zeigt Dateien und Ordner an
ls -l       # zeigt Details wie Rechte, Größe und Datum
ls -la      # zeigt auch versteckte Dateien an
```

## 📁 Verzeichnis wechseln

### `cd`

Wechselt in ein anderes Verzeichnis.

```bash
cd /etc     # wechselt in den Ordner /etc
cd ~        # wechselt ins Home-Verzeichnis
cd ..       # geht eine Ebene zurück
```

## 📍 Aktuellen Pfad anzeigen

### `pwd`

```bash
pwd         # zeigt den aktuellen Ordnerpfad an
```

## 🗂️ Ordner erstellen

### `mkdir`

```bash
mkdir test          # erstellt den Ordner test
mkdir projekt       # erstellt den Ordner projekt
```

## 📄 Datei erstellen

### `touch`

```bash
touch datei.txt     # erstellt eine leere Datei
```

## 📋 Dateien kopieren

### `cp`

```bash
cp datei.txt backup.txt     # kopiert eine Datei
cp -r ordner ziel           # kopiert einen ganzen Ordner
```

## ✏️ Dateien verschieben oder umbenennen

### `mv`

```bash
mv alt.txt neu.txt          # benennt eine Datei um
mv datei.txt /tmp           # verschiebt eine Datei nach /tmp
```

## 🗑️ Dateien löschen

### `rm`

```bash
rm datei.txt        # löscht eine Datei
rm -r ordner        # löscht einen Ordner mit Inhalt
```

## 🔍 Text suchen

### `grep`

```bash
grep "test" datei.txt       # sucht das Wort test in der Datei
grep -i "linux" datei.txt   # sucht ohne Groß- und Kleinschreibung
```

## 🔎 Dateien suchen

### `find`

```bash
find /home -name "*.txt"    # sucht alle .txt-Dateien im Ordner /home
find /tmp -type f           # sucht nur Dateien im Ordner /tmp
```

## 🔐 Rechte ändern

### `chmod`

```bash
chmod 755 skript.sh         # setzt bestimmte Rechte
chmod +x skript.sh          # macht ein Skript ausführbar
```

## 👤 Besitzer ändern

### `chown`

```bash
sudo chown max datei.txt    # ändert den Besitzer der Datei
```

## 📦 Archiv erstellen oder entpacken

### `tar`

```bash
tar -czf archiv.tar.gz ordner    # erstellt ein Archiv
tar -xzf archiv.tar.gz           # entpackt ein Archiv
```

## 🕘 Befehlsverlauf anzeigen

### `history`

```bash
history                  # zeigt alte Befehle an
history | grep git       # sucht git-Befehle im Verlauf
```

## ⚡ Abkürzungen erstellen

### `alias`

```bash
alias ll='ls -la'        # erstellt eine Abkürzung für ls -la
```

## 🔗 Pipes und Umleitungen

```bash
ls -la | grep ".txt"        # filtert die Ausgabe nach .txt-Dateien
echo "Hallo" > datei.txt    # schreibt Text in eine Datei
cat datei.txt >> ausgabe.txt # hängt Inhalt an eine Datei an
```
