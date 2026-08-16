# TheCrazyBot – Rechtliches

Statische Webseite mit Datenschutzerklärung und Nutzungsbedingungen für TheCrazyBot, gedacht zum Hosten via GitHub Pages.

## Struktur

```
index.html                 Startseite mit Links zu beiden Dokumenten
datenschutz.html            Datenschutzerklärung
nutzungsbedingungen.html    Nutzungsbedingungen
assets/style.css            Gemeinsames Stylesheet
```

## In GitHub Pages veröffentlichen

1. Neues **öffentliches** Repo auf GitHub erstellen (z. B. `thecrazybot-docs`).
2. Diese Dateien 1:1 ins Repo-Root pushen (nicht in einen Unterordner, außer du passt die Pfade in den HTML-Dateien an).
3. Im Repo zu **Settings → Pages** gehen.
4. Unter **Build and deployment** → **Source**: `Deploy from a branch` wählen.
5. **Branch**: `main`, Ordner `/ (root)` → **Save**.
6. Nach ca. 1–2 Minuten ist die Seite erreichbar unter:
   `https://<dein-github-username>.github.io/<repo-name>/`
