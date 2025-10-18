# SPD Langenselbold – 135 Jahre im Zeitstrahl

Interaktiver vertikaler Zeitstrahl zur Geschichte der SPD Langenselbold von 1863 bis heute.

## 🎯 Features

- **Chronologische Navigation**: Von der Arbeiterbewegung 1863 bis zur Gegenwart
- **Filterbare Events**: Nach Typ (Kontext, Ereignis, Person, Projekt) und thematischen Tags
- **Volltextsuche**: Durchsuche alle Ereignisse, Personen und Orte in Echtzeit
- **Responsive Design**: Optimiert für Desktop, Tablet und Mobile
- **Barrierearm**: Semantisches HTML, Tastaturnavigation, ARIA-Labels
- **Deep-Linking**: Direkte Links zu einzelnen Jahren via URL-Hash

## 🚀 Live-Demo

**[https://cbraunfi.github.io/SPD135Timeline/](https://cbraunfi.github.io/SPD135Timeline/)**

## 📦 Lokale Installation

```bash
# Repository klonen
git clone https://github.com/CBraunFI/SPD135Timeline.git
cd SPD135Timeline

# Mit einem lokalen Webserver öffnen (z.B. Python)
python -m http.server 8000

# Oder mit Node.js
npx serve .
```

Dann im Browser: `http://localhost:8000`

## 📚 Datenquellen

- Chronik SPD Langenselbold (diverse Abschnitte 1887–1990)
- Festschriften 70/90/100 Jahre SPD Langenselbold
- Wikipedia: Geschichte der SPD, Geschichte Deutschlands, Geschichte Hessens

## 🛠 Technologie

- **Reine Vanilla-Technologie**: Kein Framework, kein Build-Prozess
- **HTML5 + CSS3 + JavaScript ES6**
- **Progressive Enhancement**: Funktioniert auch ohne JavaScript (Basislayout)
- **Moderne CSS-Features**: CSS-Custom-Properties, color-mix(), backdrop-filter

## 🎨 Design

- **SPD-Corporate-Identity**: Rot #E3000F
- **Typografie**: System-Font-Stack für beste Performance
- **Lesbarkeit**: max-width 68ch für optimale Zeilenlänge
- **Kontraste**: WCAG-AA-konform

## 📝 Inhalte erweitern

Events werden direkt im `<script>`-Bereich der `index.html` definiert:

```javascript
const EVENTS = [
  {
    id:"e1890-gruendung",
    year:1890,
    date:"1890",
    title:"Gründung des sozialdemokratischen Wahlvereins Langenselbold",
    type:"Ereignis",
    excerpt:"Karl Frohme spricht 'aus dem Fenster des Brauhauses'...",
    body:"Mit dem Ende des Sozialistengesetzes...",
    tags:["Gründung","Frohme","Brauhaus"],
    source:["Chronik SPD Langenselbold, 1890"],
    milestone:true
  },
  // ... weitere Events
];
```

**Felder:**
- `id`: Eindeutige ID (String)
- `year`: Jahr (Number)
- `date`: Anzeige-Datum (String, z.B. "25.04.1945" oder "1890–1892")
- `title`: Überschrift (String)
- `type`: "Kontext", "Ereignis", "Person" oder "Projekt"
- `excerpt`: Kurzzusammenfassung (String, ~1–2 Sätze)
- `body`: Ausführliche Beschreibung (String)
- `tags`: Array von Schlagworten (Array)
- `source`: Array von Quellenangaben (Array)
- `milestone`: Boolean (true = größerer roter Marker)

## 🤝 Beitragen

Korrekturen, Ergänzungen und Verbesserungen sind willkommen!

1. Fork erstellen
2. Feature-Branch anlegen (`git checkout -b feature/neue-ereignisse`)
3. Änderungen committen (`git commit -m 'Füge Ereignisse der 2000er hinzu'`)
4. Branch pushen (`git push origin feature/neue-ereignisse`)
5. Pull Request erstellen

## 📄 Lizenz

Dieses Projekt dient der historischen Dokumentation und Bildung. Die Inhalte basieren auf öffentlich zugänglichen Quellen und internen Chroniken der SPD Langenselbold.

## ✨ Credits

Entwickelt für die SPD Langenselbold mit Unterstützung von Claude Code.

---

**SPD Langenselbold** | 135 Jahre Mut, Arbeit, Gemeinschaft (1890–2025)
