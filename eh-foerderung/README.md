# 📊 EH 55 Förderung - Infografik mit Lightbox

## ✨ Was ist das?

Eine professionelle Webseite zur Präsentation der EH 55 Förderungs-Infografik mit Lightbox-Zoom-Funktion.

Perfekt für:
- E-Mail-Marketing-Kampagnen
- Newsletter
- Kundenkommunikation
- Informationsmaterial zu Fördermitteln

## 🎯 Features

✅ **Lightbox-Zoom** - Klick auf Bild = Vollbild-Ansicht mit dunklem Hintergrund
✅ **Responsive** - Funktioniert perfekt auf Handy, Tablet & Desktop
✅ **Professionelles Design** - Modernes dunkles Design mit Hover-Effekten
✅ **Einfach zu bedienen** - Keine Programmierkenntnisse nötig
✅ **Schnell** - Optimiert für schnelle Ladezeiten
✅ **Kostenlos zu hosten** - Funktioniert mit Vercel, Netlify, Cloudflare Pages

---

## 🚀 Schnellstart

### Schritt 1: Dateien vorbereiten

Erstelle folgende Ordnerstruktur:

```
eh-foerderung/
├── bild-1.html
└── bilder/
    └── EH_55_Foerderung.jpg
```

**WICHTIG:** Benenne dein Bild genau so: `EH_55_Foerderung.jpg` (ohne Umlaute, mit Unterstrichen)

### Schritt 2: Mit Vercel CLI deployen

```bash
# Vercel CLI installieren
npm install -g vercel

# In Projekt-Ordner wechseln
cd eh-foerderung

# Deployen
vercel

# Projektname eingeben: eh-55-foerderung
```

### Schritt 3: Link nutzen

Deine URL: `https://eh-55-foerderung.vercel.app/bild-1.html`

Diese kannst du in E-Mails, Newsletter oder auf Websites teilen!

---

## 📧 In E-Mails verwenden

### Variante A: Textlink

```
Klicken Sie hier für wichtige Informationen zur EH 55 Förderung:
https://eh-55-foerderung.vercel.app/bild-1.html
```

### Variante B: Vorschaubild mit Link (HTML)

```html
<a href="https://eh-55-foerderung.vercel.app/bild-1.html">
  <img src="https://eh-55-foerderung.vercel.app/bilder/EH_55_Foerderung.jpg" 
       width="400" 
       style="border-radius: 8px; border: 2px solid #4CAF50;">
</a>
<p style="font-size: 14px; color: #666;">
  Klicken Sie auf das Bild für eine vergrößerte Ansicht
</p>
```

### Variante C: Call-to-Action Button

```html
<a href="https://eh-55-foerderung.vercel.app/bild-1.html" 
   style="background: #4CAF50; color: white; padding: 14px 28px; 
          text-decoration: none; border-radius: 8px; display: inline-block; 
          font-weight: 600;">
  📊 EH 55 Förderung - Jetzt informieren
</a>
```

---

## 🔧 Texte anpassen

### Überschrift ändern

Öffne `bild-1.html` und suche nach:

```html
<h1>EH 55 Förderung</h1>
```

Ändere zu deinem gewünschten Titel.

### Haupttext ändern

Suche nach:

```html
<div class="description">
    <h2>Update Fördermittel: Budget schmilzt...</h2>
    <p>
        Der Wettlauf um die Fördermittel...
    </p>
</div>
```

Passe die Texte zwischen `<p>` und `</p>` an.

### Weitere Absätze hinzufügen

```html
<p style="margin-top: 15px;">
    Dein neuer Absatz hier...
</p>
```

---

## 🌐 Deployment-Optionen

### Option 1: Vercel CLI (Empfohlen für Updates)

```bash
# Beim ersten Mal
vercel

# Bei Textänderungen
vercel --prod
```

**Vorteile:**
- Schnellste Methode
- Einfache Updates
- Kein GitHub nötig

### Option 2: Mit GitHub + Vercel

```bash
# Repository erstellen
git init
git add .
git commit -m "EH 55 Förderung Infografik"
gh repo create eh-55-foerderung --public --source=. --push
```

Dann auf vercel.com das Repository importieren.

**Vorteile:**
- Automatische Updates bei `git push`
- Versionskontrolle
- Backup in der Cloud

### Option 3: Netlify Drag & Drop

1. Gehe zu https://app.netlify.com/drop
2. Ziehe den `eh-foerderung`-Ordner ins Fenster
3. Fertig!

---

## 🎨 Design anpassen

### Hintergrundfarbe ändern

In `bild-1.html` suche nach:

```css
body {
    background: #1a1a1a;  /* Dunkelgrau */
}
```

Ändere zu:
- Schwarz: `#000000`
- Dunkelblau: `#0a1929`
- Tragkonzept-Grün: `#4CAF50` (für Akzente)

### Textfarbe für Beschreibung

```css
.description {
    background: rgba(255, 255, 255, 0.1);  /* Halbtransparent weiß */
    color: white;
}
```

---

## 🔧 Fehlerbehebung

### Problem: Bild wird nicht angezeigt

**Lösung:**
1. Prüfe Dateinamen: **exakt** `EH_55_Foerderung.jpg` (Unterstriche!)
2. Groß-/Kleinschreibung beachten
3. Datei muss im `bilder/` Ordner liegen

### Problem: Umlaute werden als �� angezeigt

**Lösung:**
1. Datei muss als **UTF-8** gespeichert sein
2. In VS Code: Unten rechts "UTF-8" auswählen → Speichern
3. In Notepad: "Speichern unter" → Codierung: "UTF-8"

### Problem: Lightbox öffnet nicht

**Lösung:**
1. Browser-Cache leeren (Strg+Shift+R / Cmd+Shift+R)
2. In anderem Browser testen
3. JavaScript-Konsole prüfen (F12)

### Problem: Bild lädt langsam

**Lösung:**
1. Bild komprimieren: https://tinypng.com
2. Empfohlene Größe: max. 500 KB
3. Empfohlene Auflösung: 1920px Breite

---

## 📊 Tracking & Analytics (Optional)

### Google Analytics hinzufügen

Füge vor `</head>` ein:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Vercel Analytics (Einfacher)

In Vercel Dashboard:
1. Gehe zu deinem Projekt
2. "Analytics" Tab
3. "Enable Analytics"
4. ✅ Kostenlos! Zeigt Seitenaufrufe, Klicks, etc.

---

## 💡 Profi-Tipps

### SEO optimieren

Füge in `<head>` ein:

```html
<meta name="description" content="EH 55 Förderung 2026: Aktuelle Informationen zum Budget, Mythen klären und Chancen nutzen. Von TRAGKONZEPT.">
<meta property="og:title" content="EH 55 Förderung - Mythen klären und Chancen nutzen">
<meta property="og:description" content="650 Millionen Euro verbleiben - Sichern Sie sich Ihre Förderung!">
<meta property="og:image" content="https://eh-55-foerderung.vercel.app/bilder/EH_55_Foerderung.jpg">
```

**Effekt:** Beim Teilen auf Social Media erscheint ein schönes Vorschaubild!

### Mehrere Infografiken?

1. Kopiere `bild-1.html` → `bild-2.html`
2. Lade zweites Bild hoch: `bilder/Weitere_Infografik.jpg`
3. In `bild-2.html` ändere Bildpfad und Texte
4. Erstelle `index.html` als Übersichtsseite (siehe Beispiel unten)

### Übersichtsseite erstellen

Erstelle `index.html`:

```html
<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <title>EH 55 Förderung - Infomaterial</title>
</head>
<body style="font-family: Arial; max-width: 800px; margin: 50px auto; padding: 20px;">
    <h1>EH 55 Förderung - Informationsmaterial</h1>
    
    <div style="margin: 30px 0;">
        <h2>📊 Aktuelle Budgetsituation Februar 2026</h2>
        <p>Mythen klären und Chancen nutzen</p>
        <a href="bild-1.html" style="color: #4CAF50; font-weight: 600;">
            → Infografik ansehen
        </a>
    </div>
    
    <!-- Weitere Infografiken hier hinzufügen -->
</body>
</html>
```

---

## 📞 Support & Kontakt

**Bei technischen Fragen:**
- Vercel Docs: https://vercel.com/docs
- Claude Code fragen

**Bei inhaltlichen Fragen:**
- TRAGKONZEPT Team kontaktieren

---

## 📋 Checkliste vor dem Launch

- [ ] Bild heißt `EH_55_Foerderung.jpg` (keine Umlaute!)
- [ ] Bild liegt im `bilder/` Ordner
- [ ] HTML-Datei ist UTF-8 kodiert
- [ ] Texte sind angepasst
- [ ] Auf Vercel deployed
- [ ] URL getestet (Desktop & Handy)
- [ ] Lightbox funktioniert
- [ ] In Test-E-Mail eingefügt

---

## 🎉 Fertig!

Deine EH 55 Förderungs-Infografik ist jetzt:
✅ Professionell präsentiert
✅ Mobil-optimiert
✅ Mit Zoom-Funktion
✅ Bereit für E-Mails & Newsletter
✅ Kostenlos gehostet

**Viel Erfolg mit Ihrer Förderungs-Kampagne! 🚀**

---

## 🏢 Über TRAGKONZEPT

Diese Lösung wurde für TRAGKONZEPT erstellt zur professionellen Präsentation 
von Fördermittel-Informationen im Bereich Energieeffizienz und Neubau.

*Erstellt Februar 2026 | Optimiert für Vercel Hosting*
