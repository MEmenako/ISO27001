# ISO 27001 Controls Explorer - Benutzeranleitung

## Schnellstart

1. Öffnen Sie die Datei `ISO27001_Controls_Explorer.html` in Ihrem Browser
2. Das Dashboard zeigt Ihnen eine Übersicht aller 93 Controls
3. Navigieren Sie über die Sidebar oder nutzen Sie die Suchfunktion

## Features im Detail

### 1. Favoriten

**Favoriten markieren:**
- Klicken Sie auf das Stern-Symbol (☆) bei einem Control
- Der Stern wird golden (⭐) wenn favorisiert
- Favoriten werden automatisch gespeichert

**Favoriten anzeigen:**
- Klicken Sie in der Sidebar auf "⭐ Meine Favoriten"
- Im Header sehen Sie die Anzahl Ihrer Favoriten

### 2. Fortschritts-Tracking

**Status setzen:**
1. Öffnen Sie ein Control in der Detailansicht
2. Scrollen Sie zum Abschnitt "Implementierungsstatus"
3. Wählen Sie einen Status:
   - 📂 **Offen**: Noch nicht begonnen (Standard)
   - 🔄 **In Arbeit**: Gerade in Bearbeitung
   - ✅ **Erledigt**: Implementierung abgeschlossen
   - ⛔ **Nicht anwendbar**: Für Ihre Organisation nicht relevant

**Fortschritt überwachen:**
- Im Header sehen Sie einen Fortschrittsbalken
- Zeigt Prozent und Anzahl erledigter Controls
- Im Dashboard finden Sie Statistiken pro Status

**Nach Status filtern:**
- Nutzen Sie die Status-Filter-Pills unter der Suchleiste
- Oder klicken Sie im Dashboard auf eine Status-Statistik

### 3. Notizen

**Notizen hinzufügen:**
1. Öffnen Sie ein Control in der Detailansicht
2. Scrollen Sie zum Abschnitt "📝 Notizen"
3. Geben Sie Ihre Notizen ein
4. Klicken Sie auf "Notizen speichern"

**Notizen erkennen:**
- Controls mit Notizen zeigen ein 📝-Symbol in der Kartenansicht

### 4. Suche

**Einfache Suche:**
- Geben Sie einen Begriff in die Suchleiste ein
- Gefundene Begriffe werden orange hervorgehoben
- Anzahl der Suchergebnisse wird angezeigt

**Suchbereiche:**
Die Suche durchsucht:
- Control-IDs (z.B. "A.5.1")
- Titel
- Beschreibungen
- Implementierungsleitfaden
- Praxisbeispiele

### 5. Export-Funktionen

**JSON-Export (alle Daten):**
- Klicken Sie auf "💾 JSON Export"
- Exportiert alle 93 Controls mit vollständigen Daten
- Dateiname: `ISO27001_Controls_YYYY-MM-DD.json`

**Drucken:**
- Klicken Sie auf "🖨️ Drucken"
- Öffnet den Browser-Druckdialog
- Unnötige UI-Elemente werden ausgeblendet

**Fortschritt exportieren:**
- Klicken Sie auf "📊 Fortschritt exportieren"
- Exportiert Ihre Favoriten, Notizen und Status
- Dateiname: `ISO27001_Fortschritt_YYYY-MM-DD.json`

**Fortschritt importieren:**
- Klicken Sie auf "📥 Fortschritt importieren"
- Wählen Sie eine zuvor exportierte JSON-Datei
- Ihre Daten werden wiederhergestellt

### 6. Dark Mode

**Dark Mode aktivieren:**
- Klicken Sie auf den Mond-Button (🌙) im Header
- Das Design wechselt zu dunklen Farben
- Die Einstellung wird gespeichert

**Dark Mode deaktivieren:**
- Klicken Sie auf den Sonnen-Button (☀️)
- Das Design wechselt zurück zu hellen Farben

### 7. Navigation

**Sidebar:**
- Zeigt alle Kategorien und Controls
- Klicken Sie auf eine Kategorie zum Aufklappen
- Klicken Sie auf ein Control für Details

**Filter:**
- Alle (93 Controls)
- 📊 Organisatorisch
- 👥 Menschen
- 🏢 Physisch
- 💻 Technisch
- Status-Filter (Offen, In Arbeit, Erledigt, N/A)

**Zurück-zum-Anfang:**
- Button erscheint beim Scrollen (↑)
- Klicken Sie darauf für Smooth-Scroll nach oben

## Tipps & Tricks

### Workflow-Empfehlung

1. **Erste Sichtung:**
   - Gehen Sie durch alle Controls
   - Markieren Sie relevante Controls als Favoriten

2. **Planung:**
   - Filtern Sie Ihre Favoriten
   - Setzen Sie Status "In Arbeit" für aktuelle Projekte
   - Markieren Sie nicht-anwendbare Controls als "N/A"

3. **Umsetzung:**
   - Nutzen Sie Notizen für Implementierungsdetails
   - Aktualisieren Sie den Status bei Fortschritt
   - Exportieren Sie regelmäßig Ihren Fortschritt

4. **Dokumentation:**
   - Nutzen Sie den JSON-Export für Backups
   - Drucken Sie relevante Controls aus
   - Teilen Sie Fortschrittsdaten mit Kollegen

### Datensicherheit

**Alle Daten werden lokal gespeichert:**
- Im Browser's localStorage
- Keine Cloud-Synchronisation
- Keine Datenübertragung

**Backup-Empfehlung:**
- Exportieren Sie regelmäßig Ihren Fortschritt
- Speichern Sie die JSON-Datei sicher
- Importieren Sie bei Browser-Wechsel oder Neuinstallation

### Browser-Cache

**Bei Problemen:**
1. Drücken Sie Strg+Shift+R (Windows) oder Cmd+Shift+R (Mac)
2. Löschen Sie den Browser-Cache
3. Laden Sie die Seite neu

**Daten bleiben erhalten:**
- LocalStorage wird nicht durch Cache-Löschung betroffen
- Ihre Favoriten, Notizen und Status bleiben bestehen

## Keyboard-Shortcuts

- **Strg/Cmd + F**: Browser-Suche öffnen
- **Strg/Cmd + P**: Druckdialog öffnen
- **Escape**: Detail-Ansicht schließen (falls implementiert)

## Support & Feedback

Bei Fragen oder Problemen:
- Überprüfen Sie diese Anleitung
- Schauen Sie ins CHANGELOG für technische Details
- Kontaktieren Sie Ihren IT-Administrator

## Technische Anforderungen

- Moderner Browser (Chrome, Firefox, Safari, Edge)
- JavaScript aktiviert
- LocalStorage aktiviert
- Empfohlene Bildschirmauflösung: 1920x1080 oder höher

---

**Viel Erfolg bei der Implementierung von ISO 27001!**
