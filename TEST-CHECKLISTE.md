# Test-Checkliste – Schichtwaise Website

## ✅ Durchgeführte Optimierungen

### 1. SEO-Optimierung
- [x] Meta-Titel aktualisiert: "Schichtwaise – Rockband | Live-Musik & Events buchen"
- [x] Meta-Beschreibung verbessert mit Keywords
- [x] Keywords Meta-Tag hinzugefügt
- [x] Open Graph Tags erweitert (og:image:alt, og:url)
- [x] Twitter Card Meta-Tag hinzugefügt
- [x] Canonical URL gesetzt
- [x] Theme-Color für Mobile Browser
- [x] Favicon-Link hinzugefügt

### 2. Performance-Optimierung
- [x] Font-Preloading hinzugefügt
- [x] DNS-Prefetch für Google Fonts
- [x] Partikel-Animation auf mobilen Geräten reduziert (500 → 150)
- [x] Canvas-Größe auf max. 1920x1080 begrenzt
- [x] Reduced-Motion-Support für Partikel-Animation
- [x] JavaScript mit `defer` Attribut
- [x] Utility-Funktionen für besseren Code

### 3. Fehlerbehandlung
- [x] Try-Catch für .ics Datei-Erstellung
- [x] Bessere Fetch-Fehlerbehandlung mit Status-Check
- [x] Button-Disable während Formular-Submission
- [x] Benutzerfreundliche Fehlermeldungen
- [x] Finally-Block für Button-Reenable
- [x] Console-Warnings bei fehlenden Feldern

### 4. Barrierefreiheit (Accessibility)
- [x] Skip-Link zum Hauptinhalt hinzugefügt
- [x] ARIA-Labels verbessert
- [x] Focus-Styles für Tastatur-Navigation
- [x] :focus-visible für bessere Sichtbarkeit
- [x] Reduced-Motion-Support
- [x] Semantisches HTML

### 5. Buchungssystem
- [x] FormSubmit-Integration an schichtwaise@gmail.com
- [x] Automatische .ics Kalender-Datei
- [x] Formular-Validierung
- [x] Success-Nachricht nach Buchung
- [x] Button-Status während Sendung

---

## 📋 Manuelle Test-Schritte

### Browser-Tests
1. **Website öffnen**
   - Datei: `SCHICHTWAISE/index.html`
   - In Chrome, Firefox, Edge testen

2. **Visuelle Tests**
   - [ ] Hintergrundbilder wechseln korrekt
   - [ ] Partikel-Animation funktioniert
   - [ ] Band Logo wird angezeigt
   - [ ] Social Media Icons funktionieren
   - [ ] Music Player spielt Songs
   - [ ] Booking Button öffnet Modal

3. **Buchungsformular Test**
   - [ ] Modal öffnet sich
   - [ ] Formular validiert Pflichtfelder
   - [ ] .ics Datei wird heruntergeladen
   - [ ] Formular wird an schichtwaise@gmail.com gesendet
   - [ ] Success-Nachricht wird angezeigt
   - [ ] Button wird während Sendung deaktiviert

4. **Accessibility Tests**
   - [ ] Tab-Taste navigiert durch Elemente
   - [ ] Skip-Link erscheint bei Fokus
   - [ ] Focus-Ringe sind sichtbar
   - [ ] Screen Reader kann Inhalte lesen

5. **Responsive Tests**
   - [ ] Desktop (1920px)
   - [ ] Tablet (768px)
   - [ ] Mobile (375px)
   - [ ] Alle Icons klickbar
   - [ ] Text lesbar

### FormSubmit Ersteinrichtung
1. Website im Browser öffnen
2. Booking Button klicken
3. Test-Buchung ausfüllen:
   - Name: Test Kunde
   - E-Mail: test@example.com
   - Datum: Morgen
   - Uhrzeit: 18:00
4. Formular absenden
5. **WICHTIG**: schichtwaise@gmail.com prüfen
6. Aktivierungs-E-Mail von FormSubmit bestätigen
7. Danach sind Buchungen aktiv

---

## 🔧 Lighthouse Test (Chrome DevTools)

1. Chrome öffnen
2. F12 für DevTools
3. Tab "Lighthouse" wählen
4. "Analyze page load" klicken
5. Zielwerte:
   - **Performance**: ≥90
   - **Accessibility**: ≥95
   - **Best Practices**: ≥95
   - **SEO**: ≥95

---

## 📊 Erwartete Lighthouse Scores

| Kategorie | Ziel | Status |
|-----------|------|--------|
| Performance | 90+ | ✅ Optimiert |
| Accessibility | 95+ | ✅ Verbessert |
| Best Practices | 95+ | ✅ Gut |
| SEO | 95+ | ✅ Optimiert |

---

## 🐛 Bekannte Einschränkungen

1. **FormSubmit Free Tier**: 
   - Keine individuellen Bestätigungs-E-Mails
   - Nur Eingangsbestätigung möglich
   
2. **Partikel-Animation**: 
   - Deaktiviert bei Reduced-Motion-Einstellung
   - Weniger Partikel auf Mobile (Performance)

3. **Musik-Player**: 
   - Autoplay durch Browser blockiert
   - User-Interaktion erforderlich

---

## 📝 Wartungshinweise

### Musik hinzufügen
Dateien im Ordner `musik/` ablegen und im JavaScript-Array ergänzen:
```javascript
var tracks = [
  { src: "musik/Neuer-Song.mp3", title: "Schichtwaise – Neuer Song" },
];
```

### Hintergrundbilder ändern
Bilder im Ordner `images/` ablegen und Array aktualisieren:
```javascript
const images = [
  "images/neues-bild.jpg",
];
```

### Social Media Links aktualisieren
Im HTML die `href`-Attribute der Icons ändern.

---

## ✅ Abschluss-Checkliste

- [ ] Website lokal getestet
- [ ] FormSubmit aktiviert (Erste Buchung bestätigen!)
- [ ] Alle Links funktionieren
- [ ] Mobile Darstellung geprüft
- [ ] Lighthouse Score ≥90 in allen Kategorien
- [ ] Buchungssystem funktioniert live

---

**Erstellt**: 19. März 2026  
**Version**: 1.0  
**Website**: schichtwaise.de
