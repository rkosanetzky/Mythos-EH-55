# 🚀 QUICKSTART - In 5 Minuten live!

## Schritt 1: Bilder vorbereiten
- Benenne dein Bild: `EH_55_Foerderung.jpg`
- Lege es in den `bilder/` Ordner

**Wichtig:** Verwende keine Umlaute oder Leerzeichen in Dateinamen!
- ✅ Gut: `EH_55_Foerderung.jpg`
- ❌ Schlecht: `EH 55 Förderung.jpg`

## Schritt 2: Auf Vercel hochladen

### Methode 1: Vercel CLI (Empfohlen)

```bash
# 1. Node.js installieren (falls noch nicht vorhanden)
# Download: https://nodejs.org

# 2. Vercel CLI installieren
npm install -g vercel

# 3. In deinen Projekt-Ordner wechseln
cd Pfad/zu/deinem/eh-foerderung-ordner

# 4. Deployen
vercel

# 5. Fragen beantworten:
# - Project name? eh-55-foerderung
# - Which directory? ./
# - Want to modify settings? N
```

### Methode 2: Mit GitHub

```bash
cd eh-foerderung
git init
git add .
git commit -m "Erste Version"
gh repo create eh-55-foerderung --public --source=. --push
```

Dann auf vercel.com:
1. "New Project"
2. Repository auswählen: `eh-55-foerderung`
3. "Deploy" klicken

## Schritt 3: Link in E-Mail verwenden

**Beispiel-E-Mail:**
```
Sehr geehrte Damen und Herren,

anbei finden Sie wichtige Informationen zur EH 55 Förderung:

👉 https://eh-55-foerderung.vercel.app/bild-1.html

Die Grafik zeigt die aktuelle Budgetsituation und den Mythos rund um 
die EH 55 Anforderungen. Klicken Sie auf das Bild für eine vergrößerte Ansicht.

Mit freundlichen Grüßen
Ihr TRAGKONZEPT Team
```

**ODER mit Vorschaubild:**
```html
<a href="https://eh-55-foerderung.vercel.app/bild-1.html">
  <img src="https://eh-55-foerderung.vercel.app/bilder/EH_55_Foerderung.jpg" width="400">
</a>
```

---

## Was passiert beim Klick?

1. Empfänger klickt auf Link in E-Mail
2. Webseite öffnet sich mit der Förderungs-Infografik
3. Klick auf Bild → Lightbox mit Vollbild-Ansicht
4. Klick außerhalb oder ESC → Lightbox schließt sich

---

## Weitere Bilder hinzufügen?

1. Kopiere `bild-1.html` → benenne in `bild-2.html`
2. Ändere in `bild-2.html`:
   - Bildpfad: `bilder/Neues_Bild.jpg`
   - Titel: "Neuer Titel"
   - Beschreibung anpassen
3. Neues Bild in `bilder/` Ordner hochladen
4. Update deployen:
   ```bash
   vercel --prod
   ```

---

## Dateistruktur

```
eh-foerderung/
├── index.html (optional - Übersichtsseite)
├── bild-1.html (EH 55 Förderung)
└── bilder/
    └── EH_55_Foerderung.jpg
```

---

## Bei Änderungen am Text:

1. Öffne `bild-1.html` mit Editor/VS Code
2. Suche nach `<h2>` oder `<p>` Tags
3. Ändere den Text
4. Speichern
5. Neu deployen:
   ```bash
   vercel --prod
   ```

---

## Kosten?

**0€ bei Vercel** für:
- Bis 100 GB Traffic/Monat
- Unbegrenzte Bilder
- SSL-Zertifikat inklusive
- Automatische Updates

---

## Probleme?

**Umlaute werden falsch angezeigt?**
- Datei muss als UTF-8 gespeichert sein
- In VS Code: Unten rechts "UTF-8" auswählen

**Bild wird nicht angezeigt?**
- Prüfe Dateinamen: `EH_55_Foerderung.jpg` (Unterstriche, kein Umlaut!)
- Groß-/Kleinschreibung beachten

**URL ändern?**
- Vercel Dashboard → Settings → Project Name

---

**Das war's! Viel Erfolg mit der EH 55 Förderungs-Kampagne! 🎉**
