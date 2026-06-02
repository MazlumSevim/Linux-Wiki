# 👤 Benutzerverwaltung

Diese Datei enthält wichtige Befehle zur Verwaltung von Benutzern und Gruppen unter Linux.

## 🙋 Aktuellen Benutzer anzeigen

### `whoami`

```bash
whoami      # zeigt den aktuell angemeldeten Benutzer an
```

## 🆔 Benutzerinformationen anzeigen

### `id`

```bash
id          # zeigt Benutzer-ID und Gruppen an
id max      # zeigt Informationen über den Benutzer max
```

## 👥 Angemeldete Benutzer anzeigen

### `users`

```bash
users       # zeigt aktuell angemeldete Benutzer an
```

## ➕ Benutzer erstellen

### `useradd`

```bash
sudo useradd max      # erstellt den Benutzer max
sudo useradd -m max   # erstellt Benutzer mit Home-Verzeichnis
```

## 🔑 Passwort vergeben

### `passwd`

```bash
sudo passwd max   # setzt Passwort für Benutzer max
passwd            # ändert das eigene Passwort
```

## ✏️ Benutzer ändern

### `usermod`

```bash
sudo usermod -aG sudo max     # fügt Benutzer zur sudo-Gruppe hinzu
sudo usermod -l neuer alter   # ändert den Benutzernamen
```

## ❌ Benutzer löschen

### `userdel`

```bash
sudo userdel max      # löscht den Benutzer
sudo userdel -r max   # löscht Benutzer inklusive Home-Verzeichnis
```

## 👨‍👩‍👧‍👦 Gruppe erstellen

### `groupadd`

```bash
sudo groupadd entwickler   # erstellt die Gruppe entwickler
```

## 🗑️ Gruppe löschen

### `groupdel`

```bash
sudo groupdel entwickler   # löscht die Gruppe entwickler
```

## 📋 Gruppen anzeigen

### `groups`

```bash
groups       # zeigt die eigenen Gruppen an
groups max   # zeigt Gruppen des Benutzers max an
```

## 👤 Besitzer ändern

### `chown`

```bash
sudo chown max datei.txt      # ändert den Besitzer der Datei
sudo chown max:max datei.txt  # ändert Besitzer und Gruppe
```

## 👥 Gruppe einer Datei ändern

### `chgrp`

```bash
sudo chgrp entwickler datei.txt   # ändert die Gruppe einer Datei
```

## 🛡️ Administratorrechte nutzen

### `sudo`

```bash
sudo apt update                # führt Befehl als Administrator aus
sudo systemctl restart apache2 # startet einen Dienst neu
```

## 📌 Zusammenfassung

```bash
whoami     # aktueller Benutzer
id         # Benutzerinformationen
groups     # Gruppen anzeigen
sudo       # Administratorrechte
```
