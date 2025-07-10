# BandManager
Die Band-Manager-App ist eine moderne Angular-Webanwendung für Musiker und Bands, die die Organisation und Verwaltung von Songs und Setlists vereinfacht. Sie entstand während meiner 2jährigen Ausbildung. Das Backend wurde von Luca Jürgens entwickelt und in Docker-Containern gehostet.

## Inhaltsverzeichnis
- [Projektidee](#projektidee)
- [Funktionen](#funktionen)
- [Geplante Features](#geplante-features)
- [Technologien](#technologien)
- [Architektur](#architektur)
- [User Stories](#user-stories)
- [Status](#status)
- [Team](#team)
- [Lizenz](#lizenz)

## Projektidee
Ziel des Projekts ist die Entwicklung einer Anwendung zur effizienten Organisation und Verwaltung eigener Songs und Setlists für Musikbands. Der Schwerpunkt liegt auf der _Musikbibliothek_ als zentralem Modul, das als Datenbank für bandeigene Songs dient. Darüber hinaus sollen Datenschutz, Datensicherheit, Usability und eine solide technische Basis gewährleistet sein.

**Zielgruppe:**
- Musiker und Bands

**Strategische Ziele:**
- Hohe Usability & Softwareergonomie
- Gute Testabdeckung
- Nachhaltige und erweiterbare Architektur
- Datenschutz & Datensicherheit (z. B. DSGVO-konform)

## Funktionen (umgesetzte Features)

### Musikbibliothek
- Speicherung von Song-Informationen (Titel, Texte, Akkorde, Noten, Audio-Demos)
- Anzeige aller Songs in übersichtlicher Liste
- Suche und Filterung von Songs ( nach Titel, Künstler, Genre)
- CRUD-Funktionalität (Create, Read, Update, Delete) für Songs
- Responsive Design für Desktop, Tablet und Smartphone
  
### Anmerkungen und Notizen
- Hinzufügen, Bearbeiten und Löschen von Notizen zu Songs
- Anzeige von Anmerkungen in der Song-Detailansicht
- Responsives und benutzerfreundliches Interface

*(Die Features „Setlist-Erstellung“, „Gruppenverwaltung“ und Responsive Design wurden für das initiale Release _(Projektabgabe)_ aus Zeitgründen gestrichen, sind jedoch perspektivisch geplant.)*

## geplante Features
Folgende Funktionen waren für die BandManager-App vorgesehen, wurden jedoch im Proof-of-Concept noch nicht umgesetzt:

- **Responsive Design**
  - Anpassung an verschiedene Bildschirmgrößen (Desktop, Tablet, Smartphone)
  - Mobile-First-Ansatz
  - Unterstützung von Touch-Gesten

- **Formular-Validierung**
  - Vollständige Validierung aller Formulareingaben im Frontend
  - Fehlermeldungen bei fehlenden Pflichtfeldern

- **Setlist-Erstellung**
  - Erstellung und Verwaltung von Setlists für Auftritte
  - Drag-and-Drop zur Sortierung der Songs
  - Wiederverwendung gespeicherter Setlists als Vorlage

- **Gruppenverwaltung**
  - Nutzergruppen erstellen, verwalten, löschen
  - Einladungslinks für Gruppenbeitritt

- **Nutzermanagement-Frontend**
  - Frontend-Login mit JWT-Integration
  - Benutzerkonten verwalten
  - Passwort-Reset und E-Mail-Verifizierung

- **Progressive Web App (PWA)**
  - Offline-Funktionalität
  - App-ähnliche Bedienung

- **Weitere Module (langfristig)**
  - Kalender- und Terminplanung
  - Chat-Modul für Bandmitglieder
  - Lautstärkeüberwachung per Sensoren

## Technologien
- [Angular](https://angular.io/) (Standalone Components)
- TypeScript
- SCSS
- Docker (für Backend und Datenbank)
- JWT-basierte Authentifizierung war geplant, die Umsetzung im Frontend jedoch aus Zeitgründen gestrichen.
- Datenbank: relational (MySQL)

## Architektur

### Frontend
- Entwicklung mit Angular
- Moderne UI-Komponenten
Das Frontend enthält CRUD-Funktionen für Songs. Zunächst wurde ein Mock-Backend genutzt, bevor die App an die finale REST-API des Backends angebunden wurde.

### Backend
- Entwicklung von RESTful APIs für Songs (CRUD)
- Hosting in Docker-Containern
- Datenpersistenz in Container-Datenbanken
- Planung einer JWT-basierten Authentifizierung (nicht umgesetzt im Frontend)
- Verschlüsselung sensibler Daten
- Rollen- und Berechtigungssystem (geplant)

### Sicherheit & Datenschutz

- Zugriffsbeschränkungen für alle CRUD-Operationen (geplant)
- Datenverschlüsselung bei Speicherung und Übertragung
- DSGVO-Konformität
- Backup-Strategien für Daten

## Projektmanagement
Das Projekt wurde als eduScrum-Projekt konzipiert. Es wurden User Stories mit Akzeptanzkriterien für Frontend und Backend entwickelt.

### User Story 1: Song-Datenbank

> „Als Bandmitglied möchte ich alle Songs der Band in einer zentralen Datenbank speichern können, um schnellen Zugriff auf Texte, Akkorde und Noten zu haben.“

- Formulare zur Eingabe und Bearbeitung von Songinformationen
- CRUD-Funktionen für Songs
- Such- und Filterfunktionen

*(Formular-Validierung und Responsive Design waren geplant, aber nicht vollständig umgesetzt.)*

### User Story 3: Anmerkungen zu Songs

> „Als Bandmitglied möchte ich Anmerkungen und Notizen zu Songs hinterlassen können, um z. B. wichtige Hinweise für die Probe oder den Auftritt zu speichern.“

- Eingabefelder für Notizen zu Songs
- Anzeige der Anmerkungen in der Song-Detailansicht
- CRUD-Funktionalität für Notizen

*(Diese Funktion wurde aus Zeitgründen nicht umgesetzt.)*

## Status

> **Proof-of-Concept**  
> Einige Funktionen wurden entwickelt und getestet. Teile des Codes basieren auf Projektdokumentation. Responsive Design, Touch-Unterstützung und Nutzermanagement sind aktuell nicht implementiert.

## Team

- **Andrea Küllmer** – Frontend-Entwicklung (Angular, UI/UX)
- **Luca J.** – Backend-Entwicklung (API, Datenbank, Docker)
- **S. G.** – Product Owner / Mentor

  ## Screenshots
  siehe Ordner '/screenshots'

  ## Status
  Proof-of-Concept
  Code, zT rekonstruiert aus Projektdokumentation




  ## Projektmanagement
  Das Projekt wurde als edu-Scrum-Projekt konzipiert. Es wurden User Stories mit Akzeptanzkriterien für jeweils Front- und Backend.
  User Story 1: „Als Bandmitglied möchte ich alle Songs der Band in einer zentralen Datenbank speichern können, um schnellen Zugriff auf Texte, Akkorde und Noten zu haben.“
  User Story 2: „Als Bandmitglied möchte ich Anmerkungen und Notizen zu Songs hinterlassen können, um z.B. wichtige Hinweise für die Probe oder den Auftritt zu speichern.“

  ## Lizenz
  Dieses Projekt steht unter der Creative Commons Attribution-NonCommercial 4.0 Lizenz. Keine kommerzielle Nutzung erlaubt.
