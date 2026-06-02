# Linux-Befehle

Diese Datei enthält wichtige Linux-Befehle für die tägliche Arbeit im Terminal.

## ls

Zeigt den Inhalt eines Verzeichnisses an.

Beispiele:

```bash
ls
ls -l
ls -la
cd

Wechselt in ein anderes Verzeichnis.

Beispiele:

cd /etc
cd ~
cd ..
pwd

Zeigt das aktuelle Verzeichnis an.

pwd
mkdir

Erstellt neue Verzeichnisse.

mkdir test
mkdir projekt
rmdir

Löscht leere Verzeichnisse.

rmdir test
cp

Kopiert Dateien oder Ordner.

cp datei.txt backup.txt
cp -r ordner ziel
mv

Verschiebt oder benennt Dateien um.

mv alt.txt neu.txt
mv datei.txt /tmp
rm

Löscht Dateien und Ordner.

rm datei.txt
rm -r ordner
touch

Erstellt eine leere Datei.

touch datei.txt
cat

Zeigt den Inhalt einer Datei an.

cat datei.txt
grep

Sucht nach einem bestimmten Text.

grep "test" datei.txt
grep -i "linux" datei.txt
find

Sucht Dateien und Verzeichnisse.

find /home -name "*.txt"
find /tmp -type f
chmod

Ändert Dateiberechtigungen.

chmod 755 skript.sh
chmod +x skript.sh
chown

Ändert den Besitzer einer Datei.

chown max datei.txt
tar

Erstellt oder entpackt Archive.

tar -czf archiv.tar.gz ordner
tar -xzf archiv.tar.gz
history

Zeigt bereits ausgeführte Befehle an.

history
history | grep git
alias

Erstellt eigene Befehlsabkürzungen.

alias ll='ls -la'
Pipes und Umleitungen

Ausgaben von Befehlen können weitergeleitet werden.

ls -la | grep ".txt"
echo "Hallo" > datei.txt
cat datei.txt >> ausgabe.txt
