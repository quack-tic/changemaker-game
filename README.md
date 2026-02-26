# 🌍 Changemaker – Das Brettspiel

**Zeig, dass du durch eigenes Handeln positive Veränderungen bewirken kannst!**

Ein interaktives, kostenloses Brettspiel im Browser – entwickelt für Jugendliche ab 12 Jahren. Würfle dich durch die Stadt, triff Entscheidungen zu realen Alltagssituationen und sammle Impact-Punkte.

▶️ **[Jetzt spielen](https://quack-tic.github.io/changemaker-game/)**

---

## 🎯 Worum geht's?

Changemaker ist ein digitales Brettspiel, das Jugendlichen spielerisch zeigt, wie sie in ihrem Alltag positive Veränderungen bewirken können. Bei jedem Spielfeld begegnest du einer realistischen Situation – und entscheidest, wie du handelst.

Jede Entscheidung hat Konsequenzen: Mutige, engagierte Handlungen bringen viele Impact-Punkte, Wegschauen kostet welche. Wer zuerst **30 Impact-Punkte** erreicht, gewinnt.

## 🧩 Spielprinzip

| | |
|---|---|
| 👥 **Spieler** | 2–4 |
| ⏱️ **Dauer** | ca. 15–30 Minuten |
| 🎂 **Alter** | Ab 12 Jahren |
| 🎲 **Mechanik** | Würfeln → Feld betreten → Szenario lesen → Entscheidung treffen → Punkte sammeln |
| 🏆 **Ziel** | 30 Impact-Punkte erreichen |

## 🌈 Fünf Themenbereiche

| Kategorie | Felder | Beispielthemen |
|---|---|---|
| 🌱 **Umwelt** | 16 Szenarien | Plastikmüll, Fast Fashion, Energiesparen, Bienenschutz, Lebensmittelverschwendung |
| 🤝 **Soziales** | 16 Szenarien | Cybermobbing, Inklusion, Vorurteile, Obdachlosigkeit, LGBTQ+ Solidarität |
| 🏘️ **Gemeinschaft** | 15 Szenarien | Nachbarschaftshilfe, Jugendtreffs, Katastrophenhilfe, lokaler Handel |
| 📱 **Digital** | 15 Szenarien | Fake News, Datenschutz, Deepfakes, Medienkompetenz, Passwort-Sicherheit |
| ⚡ **Events** | 15 Szenarien | Rückschläge, Chancen, Überraschungen, Dilemma-Situationen |

**→ 77+ einzigartige Szenarien insgesamt**

## 🔁 Keine Wiederholungen

Das Spiel verwendet ein intelligentes Fragen-System:

- Beim Start wird jede Kategorie zufällig gemischt
- Pro Thema wird jedes Szenario erst einmal gestellt, bevor sich etwas wiederholt
- Erst wenn alle Fragen einer Kategorie durch sind, wird der Pool neu gemischt
- Der Fortschritt wird unten im Spiel angezeigt

Das bedeutet: Auch bei 4 Spielern und mehreren Runden erlebt ihr immer neue Situationen.

## 🚀 Selbst hosten

### GitHub Pages (empfohlen)

1. Repository forken oder erstellen
2. `index.html` hochladen
3. **Settings → Pages → Source: Deploy from branch → main → / (root) → Save**
4. Nach 1–2 Minuten live unter `https://Username.github.io/changemaker-game/`

### Lokal spielen

Einfach die `index.html` im Browser öffnen – fertig. Keine Installation, kein Server, keine Abhängigkeiten.

## 🛠️ Technik

- **Reine HTML/CSS/JS** – keine Frameworks, keine Build-Tools, keine Abhängigkeiten
- **Eine einzige Datei** – alles in `index.html`
- **Offline-fähig** – funktioniert ohne Internet (nach erstem Laden der Schriftarten)
- **Responsiv** – funktioniert auf Desktop, Tablet und Smartphone
- **Keine Cookies, kein Tracking, keine Datenerhebung**

## 📚 Pädagogischer Hintergrund

Das Spiel wurde für den Einsatz in Schulen, Jugendgruppen und der außerschulischen Bildung entwickelt. Es eignet sich besonders für:

- **Ethik- und Sozialkundeunterricht** – Alltagssituationen diskutieren
- **Projekttage** zu Nachhaltigkeit und Engagement
- **Jugendarbeit** – spielerischer Einstieg in gesellschaftliche Themen
- **Medienkompetenz-Workshops** – digitale Verantwortung thematisieren

Jedes Szenario bietet drei Handlungsoptionen mit unterschiedlichem Engagement-Level. Das Feedback erklärt sachlich, warum eine Entscheidung gut oder schlecht war – ohne zu moralisieren.

## 📝 Eigene Szenarien hinzufügen

Die Szenarien sind im JavaScript-Objekt `SCENARIOS` definiert. Neue Fragen lassen sich einfach ergänzen:

```javascript
{
  title: 'Titel des Szenarios',
  story: 'Beschreibung der Situation...',
  choices: [
    { text: '🌟 Beste Option', points: 4, feedback: 'Positives Feedback', level: 'good' },
    { text: '👍 Mittlere Option', points: 2, feedback: 'Neutrales Feedback', level: 'ok' },
    { text: '😐 Schlechte Option', points: -1, feedback: 'Erklärendes Feedback', level: 'bad' }
  ]
}
```

## 📄 Lizenz

Frei nutzbar für Bildungszwecke. Bei Weiterentwicklung freuen wir uns über einen Link zurück zu diesem Repository.

---

> *„Sei du selbst die Veränderung, die du dir wünschst für diese Welt."*
