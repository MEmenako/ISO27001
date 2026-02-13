# ISO 27001 Controls Explorer - Changelog

## Version 2.0 - Erweiterte Funktionalitäten (2026-02-13)

### Neue Features

#### 1. Export-Funktionen
- **JSON-Export**: Export aller Controls mit vollständigen Daten
  - Exportiert Controls, Favoriten, Notizen und Status
  - Dateiname enthält aktuelles Datum
  - Format: `ISO27001_Controls_YYYY-MM-DD.json`

- **Druckfreundlicher Export**: Optimierte Druckansicht
  - Button zum Auslösen des Druckdialogs
  - Print-CSS versteckt unnötige UI-Elemente
  - Seitenumbrüche bei Control-Cards vermieden

- **Fortschritt exportieren/importieren**:
  - Export der Fortschrittsdaten (Favoriten, Notizen, Status)
  - Import-Funktion zum Wiederherstellen der Daten
  - Dateiname: `ISO27001_Fortschritt_YYYY-MM-DD.json`

#### 2. Favoriten/Lesezeichen
- **Stern-Icon bei jedem Control**: Klickbarer Stern (☆/⭐)
  - Auf Control-Cards in der Listenansicht
  - In der Detailansicht (größer dargestellt)
- **LocalStorage-Persistenz**: Favoriten bleiben nach Neuladen erhalten
- **Favoriten-Filter**: Eigene Kategorie "Meine Favoriten" in der Sidebar
- **Favoriten-Zähler**: Anzeige im Header (⭐ Anzahl)
- **Sidebar-Integration**: Favoriten-Kategorie mit Badge oben in der Sidebar

#### 3. Fortschritts-Tracking
- **Status-Buttons für jedes Control**:
  - 📂 Offen (Standard)
  - 🔄 In Bearbeitung
  - ✅ Erledigt
  - ⛔ Nicht anwendbar

- **Fortschrittsbalken im Header**:
  - Zeigt Prozent der erledigten Controls
  - Zeigt Anzahl (z.B. "42% (39/93)")
  - Grüner Balken mit Animation

- **Status-Filter**: Filterung nach Status über Pill-Buttons
  - Eigene Filter-Pills für jeden Status
  - Anzeige der Anzahl pro Status

- **Status-Statistiken im Dashboard**:
  - Vier neue Stat-Cards mit Anzahl pro Status
  - Klickbar für direktes Filtern

- **Status-Indikatoren auf Cards**:
  - Kleines Badge unten rechts auf jeder Card
  - Farbcodiert nach Status

#### 4. Notizen-Funktion
- **Notizen-Bereich in Detailansicht**:
  - Textfeld für freie Notizen zu jedem Control
  - "Notizen speichern"-Button
  - LocalStorage-Persistenz

- **Notizen-Indikator (📝)**:
  - Erscheint auf Control-Cards wenn Notizen vorhanden
  - Tooltip "Notizen vorhanden"

#### 5. Verbesserte Suche
- **Such-Highlighting**:
  - Gefundene Begriffe werden orange hervorgehoben
  - Highlighting in Titel und Text-Preview
  - CSS-Klasse: `.search-highlight`

- **Erweiterte Suchbereiche**:
  - Suche auch in Examples (Praxisbeispiele)
  - Suche in Guidance (Implementierungsleitfaden)
  - Suche in Purpose (Zweck)

- **Suchergebniszähler**:
  - Anzeige "Suchergebnisse für "Begriff" (X Treffer)"

#### 6. Zusätzliche Features

##### Zurück-zum-Anfang Button
- Button erscheint beim Scrollen (ab 300px)
- Fixiert unten rechts (↑)
- Smooth-Scroll-Animation
- mib-Farbschema (#C0143C)

##### Dark Mode
- Toggle-Button im Header (🌙/☀️)
- Vollständiges dunkles Theme
- LocalStorage-Persistenz der Einstellung
- Angepasste Farben für alle UI-Elemente

##### Export/Import-Leiste
- Eigene Leiste unter der Suchleiste
- Vier Buttons für verschiedene Export-Funktionen
- Icon-Buttons mit klaren Beschriftungen

### Technische Details

#### LocalStorage-Keys
- `iso27001_favorites`: Favoriten (Object mit Control-IDs)
- `iso27001_notes`: Notizen (Object mit Control-ID -> Text)
- `iso27001_statuses`: Status (Object mit Control-ID -> Status)
- `iso27001_darkMode`: Dark Mode aktiviert (String "0" oder "1")

#### CSS-Anpassungen
- Neue Klassen für Favoriten, Status, Notizen
- Dark Mode Styles für alle Komponenten
- Responsive Anpassungen beibehalten
- Print-Styles erweitert

#### JavaScript-Funktionen (Neu)
- `loadFromStorage()`: Lädt Daten aus localStorage
- `saveFavorites()`, `saveNotes()`, `saveStatuses()`: Speichert Daten
- `toggleFavorite(id, event)`: Favorit hinzufügen/entfernen
- `showFavorites()`: Zeigt nur Favoriten an
- `updateFavCount()`: Aktualisiert Favoriten-Zähler
- `saveControlNote(id)`: Speichert Notiz zu einem Control
- `setStatus(id, status)`: Setzt Status eines Controls
- `updateProgress()`: Aktualisiert Fortschrittsbalken
- `exportAsJSON()`: Exportiert alle Daten als JSON
- `exportToPrint()`: Öffnet Druckdialog
- `exportProgress()`: Exportiert nur Fortschrittsdaten
- `importProgress()`: Importiert Fortschrittsdaten
- `handleImportFile(input)`: Verarbeitet Import-Datei
- `toggleDarkMode()`: Schaltet Dark Mode um
- `loadDarkMode()`: Lädt Dark Mode Einstellung
- `scrollToTop()`: Scrollt zum Anfang
- `handleScroll()`: Zeigt/versteckt Scroll-Button
- `highlightText(text, query)`: Hebt Suchbegriffe hervor
- `filterByStatus(status)`: Filtert Controls nach Status

### Farbschema (mib)
- Hauptfarbe: #C0143C (Rot)
- Sekundärfarbe: #8B0F2C (Dunkelrot)
- Türkis: #00677F
- Orange: #EF8200
- Grau: #616265

### Kompatibilität
- Alle modernen Browser (Chrome, Firefox, Safari, Edge)
- LocalStorage erforderlich für Persistenz
- JavaScript erforderlich für alle Funktionen
- Responsive Design für Mobile/Tablet/Desktop

### Backup
- Originaldatei gesichert als: `ISO27001_Controls_Explorer_backup.html`

---

## Version 1.0 - Initiale Version
- 93 ISO 27001:2022 Controls
- Kategorien: Organisatorisch, Menschen, Physisch, Technisch
- Dashboard mit Statistiken
- Filterung nach Kategorien
- Suchfunktion
- Detailansicht für jedes Control
- Responsive Design
- mib-Farbschema
