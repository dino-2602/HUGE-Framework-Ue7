#Huge Framework – Benutzerverwaltung mit Gruppen und jQuery DataTables

## Übersicht
Dieses Projekt erweitert das Huge Framework um folgende Funktionen:
- Benutzergruppenverwaltung: Einführung von Benutzergruppen mit spezifischen Rechnten.
- Interaktive Benutzerliste: Darstellung aller Benutzer und ihrer Gruppen in einer interaktiven Tabelle mittels jQuerry DataTables.

## Features
- **Benutzergruppen: Zuordnung von Benutzern zu definierten Gruppen wie Admin, Gast und regulärer Benutzer.
- **Admin-Funktionalität: Administratoren können Benutzer erstellen, bearbeiten und Gruppen zuweisen.
- **Interaktive Tabellen: Nutzung von jQuery DataTables für eine dynamische und durchsuchbare Benutzerliste.

## Technologien
![PHP](https://img.shields.io/badge/PHP-7.4%2B-blue?logo=php&logoColor=white)
![Huge Framework](https://img.shields.io/badge/Huge_Framework-1.0-brightgreen)
![HTML](https://img.shields.io/badge/HTML-5-orange?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-3-blue?logo=css3&logoColor=white)
![PHPStorm](https://img.shields.io/badge/IDE-PHPStorm-purple?logo=phpstorm&logoColor=white)
![MySQL](https://img.shields.io/badge/Database-MySQL-lightblue?logo=mysql&logoColor=white)

⚠️**Hinweis:** In diesem Repository wurde ausschließlich der `application`-Ordner hochgeladen. Dies geschieht, um den Datenschutz zu gewährleisten und keine sensiblen Daten wie Serverkonfigurationen oder Zugangsdaten öffentlich bereitzustellen. Dateien wie `config.php` und andere Konfigurationsdateien, die möglicherweise sensible Informationen enthalten, wurden absichtlich nicht hochgeladen.

## Schritte zur Implementierung

1. **Datenbankanpassungen:**
   - Erstellung einer groups-Tabelle zur Definition von Benutzergruppen.
   - Hinzufügen eines group_id-Feldes zur users-Tabelle zur Verknüpfung mit der groups-Tabelle.
  
2. **Backend-Änderungen:**
   - Aktualisierung der Benutzerverwaltungslogik, um die Zuweisung von Gruppen zu unterstützen.
   - Implementierung von Berechtigungsprüfungen basierend auf Benutzergruppen.
  
3. **Frontend-Integration:**
   - Einbindung von jQuery und DataTables für eine interaktive Benutzerliste.
   - Erstellung von Admin-Ansichten zur Verwaltung von Benutzern und deren Gruppenzuweisungen.

## Screenshots

 **Datenbankstruktur: Benutzergruppen**

![Datenbankstruktur](https://github.com/dino-2602/HUGE-Framework-Ue7/blob/main/sceenshots/db_groups.png)
- Die Datenbanktabelle user_groups definiert die verfügbaren Benutzergruppen. Jede Gruppe hat eine eindeutige group_id und einen Namen (group_name). Diese Tabelle wird verwendet, um Benutzer mit spezifischen Gruppenrollen zu verknüpfen.

**Benutzerübersicht und Dropdown-Menü zur Gruppenzuweisung**

![Benutzerübersicht und Dropdown-Menü zur Gruppenzuweisung](https://github.com/dino-2602/HUGE-Framework-Ue7/blob/main/sceenshots/admin_procon.png)
- Die Benutzerübersicht zeigt eine Liste aller Benutzer im System, einschließlich ihrer ID, Avatar, E-Mail-Adresse und zugewiesenen Gruppenrollen. Das Dropdown-Menü erlaubt es Administratoren, Benutzer zu einer der definierten Gruppen (Admin, Gast, Normaler Benutzer) zuzuweisen. Änderungen können mit dem "Submit"-Button gespeichert werden.

**HTML-Code des Dropdown-Menüs**

![HTML-Code des Dropdown-Menüs](https://github.com/dino-2602/HUGE-Framework-Ue7/blob/main/sceenshots/userrole_dropdown.png)
- Das Dropdown-Menü wird dynamisch mit PHP generiert. Die aktuelle Benutzergruppe wird basierend auf der group_id vorausgewählt. Hier ist ein Ausschnitt aus dem Code, der das Dropdown-Menü erstellt und die Gruppenoptionen dynamisch aus der Datenbank lädt.
 
## Installation
1. Klone dieses Repository:
   ```bash
   git clone https://github.com/dino-2602/HUGE-Framework-Ue7.git
