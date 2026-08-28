# TheCrazyBot – Rechtliches

Dieses Repository enthält die Datenschutzerklärung und die Nutzungsbedingungen für die Discord-App **TheCrazyBot**, veröffentlicht als statische Webseite auf GitHub Pages.

🔗 **Live:** https://marcel1853.github.io/thecrazybot-docs/
🇩🇪 Deutsch (Standard) · 🇬🇧 [English](https://marcel1853.github.io/thecrazybot-docs/en/)

## Worum geht's

TheCrazyBot ist eine Multi-Feature-Discord-App (Moderation, Ticket-System, Leveling, Economy, temporäre Sprachkanäle u. a.). Diese Seite dokumentiert transparent, welche Nutzerdaten die App verarbeitet, zu welchem Zweck, und wie Nutzer ihre Rechte nach der DSGVO wahrnehmen können – unter anderem direkt über den `/privacy`-Slash-Command in der App selbst (Auskunft, Export, Löschung).

Die Inhalte sind bewusst kein generischer Rechtstext, sondern spiegeln die tatsächlichen Funktionen und Datenmodelle des App-Codes wider.

## Seitenstruktur

| Datei | Inhalt |
|---|---|
| `index.html` | Startseite (DE) |
| `datenschutz.html` | Datenschutzerklärung (DE) |
| `nutzungsbedingungen.html` | Nutzungsbedingungen (DE) |
| `en/index.html` | Landing page (EN) |
| `en/privacy.html` | Privacy Policy (EN) |
| `en/terms.html` | Terms of Service (EN) |
| `assets/css/style.css` | Gemeinsames Stylesheet für alle Seiten |
| `.github/workflows/deploy.yml` | CI/CD-Pipeline für GitHub Pages |

Reines HTML/CSS, kein Build-Schritt, keine Abhängigkeiten – jede Seite ist direkt im Browser lauffähig.

## Wie es deployt wird

Ein GitHub-Actions-Workflow (`.github/workflows/deploy.yml`) läuft bei jedem Push auf `main`:

1. **Check-Job** – prüft, ob alle Pflichtseiten (DE + EN) und der `assets/`-Ordner vorhanden sind. Bricht bei fehlenden Dateien ab, bevor irgendetwas deployt wird.
2. **Deploy-Job** – kopiert die HTML-Seiten, `assets/` und `en/` in einen `dist/`-Ordner und veröffentlicht ihn auf dem Branch `gh-pages`.

GitHub Pages muss dafür in den Repo-Einstellungen auf **Source: Deploy from a branch → `gh-pages` → `/ (root)`** stehen.

## Für eigene Projekte nachnutzen

Wer diese Struktur für eine eigene App/eigene Seite übernehmen möchte:

1. Repo forken oder als Vorlage nutzen.
2. In den HTML-Dateien App-Name, Befehle, Kontaktdaten und die Datentabellen in Abschnitt 3 der Datenschutzerklärung anpassen.
3. Farben/Schriften lassen sich zentral über die CSS-Variablen am Anfang von `assets/css/style.css` ändern.
4. `README.md` und Workflow-Datei können unverändert übernommen werden.

## Rechtlicher Hinweis

Die Texte sind auf Basis der tatsächlichen App-Funktionen erstellt, ersetzen aber keine individuelle Rechtsberatung. Bei eigener Nutzung sollten sie an die jeweilige Situation angepasst und im Zweifel juristisch geprüft werden.

Der Verantwortliche gemäß Abschnitt 1 der Datenschutzerklärung ergänzt Name und ladungsfähige Anschrift zu einem späteren Zeitpunkt.
