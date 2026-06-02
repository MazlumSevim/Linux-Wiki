# Benutzerverwaltung

Diese Datei enthält wichtige Befehle zur Verwaltung von Benutzern und Gruppen unter Linux.

## whoami

Zeigt den aktuell angemeldeten Benutzer an.

```bash
whoami
id

Zeigt Informationen über einen Benutzer an.

id
id max
users

Zeigt aktuell angemeldete Benutzer an.

users
useradd

Erstellt einen neuen Benutzer.

sudo useradd max
sudo useradd -m max
passwd

Vergibt oder ändert ein Passwort.

sudo passwd max
passwd
usermod

Ändert Einstellungen eines Benutzers.

sudo usermod -aG sudo max
sudo usermod -l neuername altername
userdel

Löscht einen Benutzer.

sudo userdel max
sudo userdel -r max
groupadd

Erstellt eine neue Gruppe.

sudo groupadd entwickler
groupdel

Löscht eine Gruppe.

sudo groupdel entwickler
groups

Zeigt die Gruppen eines Benutzers an.

groups
groups max
chown

Ändert den Besitzer einer Datei.

sudo chown max datei.txt
sudo chown max:max datei.txt
chgrp

Ändert die Gruppe einer Datei.

sudo chgrp entwickler datei.txt
sudo

Führt Befehle mit Administratorrechten aus.

sudo apt update
sudo systemctl restart apache2
Benutzerinformationen anzeigen
whoami
id
groups
Benutzer erstellen und Passwort vergeben
sudo useradd -m max
sudo passwd max
Benutzer löschen
sudo userdel -r max
