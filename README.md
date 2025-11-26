# Merten Instabus 6227 Label Editor

Ein webbasierter Editor zur Erstellung von benutzerdefinierten Etiketten für Merten Instabus 6227 Multifunktionsschalter.

![Merten 6227 Label Editor](screenshot.png)

## 📋 Übersicht

Der Merten Instabus 6227 ist ein KNX-Multifunktionsschalter mit 8 programmierbaren Tastern (4 links, 4 rechts). Dieser Editor ermöglicht es, professionelle Beschriftungsetiketten für die mittlere Aussparung des Schalters zu erstellen.

## ✨ Features

- 🏷️ **Multi-Label-Editor**: Erstelle mehrere Etiketten gleichzeitig
- 🎨 **33 vordefinierte Symbole**: Glühbirne, Ventilator, Schloss, Tür, und viele mehr
- ✏️ **Frei editierbar**: Alle Raumnamen und Symbole individuell anpassbar
- 📐 **Korrekte Maße**: Exakt 32 mm × 47 mm (3,2 cm × 4,7 cm)
- 🖨️ **Druckfertig**: Optimiert für Selbstklebeetiketten
- 👁️ **Live-Vorschau**: Änderungen werden sofort angezeigt
- ☑️ **Zeilen aktivieren/deaktivieren**: Für teilweise konfigurierte Schalter
- 🌐 **Offline nutzbar**: Keine Internetverbindung erforderlich

## 🚀 Installation

1. Repository klonen oder herunterladen:
```bash
git clone https://github.com/DEIN-USERNAME/merten-6227-label-editor.git
cd merten-6227-label-editor
```

2. Die Datei `merten_label_editor.html` im Browser öffnen
   - Einfach doppelklicken oder
   - Mit einem lokalen Webserver öffnen

## 📁 Projektstruktur

```
merten-6227-label-editor/
├── merten_label_editor.html    # Haupt-Editor-Datei
├── Symbols/                     # Ordner mit allen Symbol-Icons
│   ├── symbol1.png             # Power-Symbol
│   ├── symbol15.png            # Glühbirne
│   ├── symbol20.png            # Ventilator
│   └── ...                     # 33 Symbole insgesamt
└── README.md                   # Diese Datei
```

## 🎯 Verwendung

### Schritt 1: Editor öffnen
Öffne `merten_label_editor.html` in einem modernen Webbrowser (Chrome, Firefox, Edge, Safari).

### Schritt 2: Etiketten erstellen
1. **Neues Etikett hinzufügen**: Klicke auf "➕ Neues Etikett hinzufügen"
2. **Namen vergeben**: Gib dem Etikett einen Namen (z.B. "Wohnzimmer", "1. OG")
3. **Zeilen konfigurieren**:
   - Gib Raumnamen ein (z.B. "Bad", "Gang", "Küche")
   - Wähle passende Symbole aus dem Dropdown
   - Deaktiviere nicht benötigte Zeilen mit der Checkbox
4. **Vorschau prüfen**: Die Änderungen werden automatisch in der Vorschau angezeigt

### Schritt 3: Drucken
1. Klicke auf "🖨️ Alle Etiketten drucken"
2. Im Druckdialog:
   - Wähle **"Tatsächliche Größe"** oder **"100% Skalierung"**
   - Deaktiviere **"An Seite anpassen"**
3. Drucke auf selbstklebende Etikettenfolie oder normales Papier
4. Schneide entlang der gestrichelten Linien aus

## 📐 Technische Spezifikationen

- **Etikett-Maße**: 32 mm × 47 mm (3,2 cm × 4,7 cm)
- **Zeilen pro Etikett**: 4 (jeweils 11,75 mm hoch)
- **Symbol-Format**: PNG, optimiert für 5-6 mm Höhe
- **Schriftgröße**: 2,5 mm für optimale Lesbarkeit
- **Layout**: EIN - [Symbol] - AUS pro Zeile

## 🎨 Verfügbare Symbole

Der Editor enthält 33 vordefinierte Symbole:

| Kategorie | Symbole |
|-----------|---------|
| **Licht** | Glühbirne, Sonne, Mond |
| **Steuerung** | Power, Plus, Minus, Pfeile |
| **Geräte** | Ventilator, Heizung, Lautsprecher, Monitor |
| **Sicherheit** | Schloss, Schlüssel, Auge, Tür |
| **Sonstiges** | Glocke, Uhr, Musik, Einstellungen, Haus |

## 🛠️ Anpassungen

### Eigene Symbole hinzufügen

1. Erstelle PNG-Bilder mit transparentem Hintergrund
2. Empfohlene Größe: 300x300 Pixel
3. Speichere sie im `Symbols/`-Ordner als `symbol34.png`, `symbol35.png`, etc.
4. Füge im HTML-Code im `symbols`-Array neue Einträge hinzu:

```javascript
const symbols = [
    // ... bestehende Symbole
    { file: 'symbol34.png', name: '🆕 Dein Symbol' }
];
```

## 🖨️ Druck-Tipps

### Empfohlene Materialien
- **Selbstklebende Etikettenfolie**: Weiß, matt oder glänzend
- **Papierformat**: A4
- **Drucker**: Tintenstrahl oder Laser

### Druckeinstellungen
- **Qualität**: Höchste Qualität / Fotoqualität
- **Skalierung**: 100% / Tatsächliche Größe
- **Ausrichtung**: Hochformat
- **Ränder**: Standard

### Nach dem Druck
1. Schneide entlang der gestrichelten Linien
2. Teste die Passform am Schalter
3. Reinige die Schalteroberfläche vor dem Aufkleben
4. Klebe das Etikett mittig auf

## 🔧 Systemanforderungen

- **Browser**: Moderner Webbrowser mit JavaScript-Unterstützung
  - Chrome 90+
  - Firefox 88+
  - Safari 14+
  - Edge 90+
- **Betriebssystem**: Windows, macOS, Linux
- **Drucker**: Beliebiger Drucker mit A4-Unterstützung

## 📝 Lizenz

Dieses Projekt ist unter der MIT-Lizenz lizenziert - siehe [LICENSE](LICENSE) Datei für Details.

## 🤝 Beiträge

Beiträge sind willkommen! Hier sind einige Möglichkeiten, wie du helfen kannst:

- 🐛 Fehler melden
- 💡 Neue Features vorschlagen
- 🎨 Neue Symbole hinzufügen
- 📖 Dokumentation verbessern
- 🌍 Übersetzungen hinzufügen

### Pull Requests
1. Forke das Repository
2. Erstelle einen Feature-Branch (`git checkout -b feature/NeuesFeature`)
3. Committe deine Änderungen (`git commit -m 'Neues Feature hinzugefügt'`)
4. Pushe zum Branch (`git push origin feature/NeuesFeature`)
5. Öffne einen Pull Request

## 📧 Kontakt & Support

- **Issues**: Nutze die GitHub Issues für Fehlerberichte und Feature-Requests
- **Diskussionen**: GitHub Discussions für allgemeine Fragen

## ⚙️ Kompatibilität

Getestet mit:
- ✅ Merten Instabus 6227 Multifunktionsschalter
- ✅ Verschiedene Browser (Chrome, Firefox, Safari, Edge)
- ✅ Windows 10/11, macOS, Linux

## 🎯 Roadmap

Geplante Features:
- [ ] Export als PDF
- [ ] Vorlagen-Bibliothek für häufige Räume
- [ ] Mehrsprachige Unterstützung (EN, DE, FR)
- [ ] Dark Mode
- [ ] Symbol-Upload-Funktion
- [ ] QR-Code-Integration für digitale Dokumentation

## 📚 Weiterführende Links

- [Merten Produktseite](https://www.merten.de)
- [KNX Standard](https://www.knx.org)
- [Instabus EIB/KNX](https://de.wikipedia.org/wiki/KNX-Standard)

## 👏 Danksagungen

- Icons/Symbole: Eigene Erstellung oder lizenzfreie Quellen
- Merten/Schneider Electric für die Entwicklung des 6227 Schalters

## 📄 Changelog

### Version 1.0.0 (2024-11-26)
- ✨ Initiales Release
- 🏷️ Multi-Label-Editor
- 🎨 33 vordefinierte Symbole
- 🖨️ Druckfunktion mit korrekten Maßen
- ✏️ Frei editierbare Etiketten

---

**Hinweis**: Dieses Projekt ist nicht offiziell mit Merten oder Schneider Electric verbunden.