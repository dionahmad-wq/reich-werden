# Projekt: Dions Webdesign

## Worum es geht

Ich (Dion) betreibe ein kleines Webdesign-Unternehmen unter dem Namen **Webdesign Salzgitter**.
Ich baue Webseiten für Kunden und verkaufe sie als feste Pakete.
Dieses Repo enthält meine eigene Firmen-Webseite (https://salzgitter-webdesign.de),
Beispielseiten für Kundenprojekte und meinen Vermögens- & Zakat-Rechner.

## Ziel

- Kunden gewinnen und Pakete verkaufen
- Meine Webseite soll Vertrauen schaffen und zu einer Anfrage führen (Kontaktformular, E-Mail, Instagram-DM)

## Zielgruppe

- Kleine Läden und Betriebe in **ganz Deutschland** (Schwerpunkt und persönliche Treffen: Salzgitter/Braunschweig):
  Barbershops, Dönerläden/Imbisse, Bäckereien, Friseure, Moscheegemeinden, Nachhilfe, Handwerker
- Auftritt: „Aus Salzgitter. Für ganz Deutschland.“ Name und Domain bleiben „Webdesign Salzgitter“
- Zusammenarbeit läuft online (E-Mail, Instagram, Videocall). Telefonnummer wird nicht veröffentlicht
- Die meisten öffnen die Seite auf dem Handy
- Stil: cool, modern, street-mäßig – NICHT technisch oder steif
- Kurze Texte, klare Sprache, Du-Ansprache, keine Werbefloskeln

## Meine Pakete

- **Starter – 149 € einmalig:** einseitige Webseite mit Infos, Öffnungszeiten, Kontakt & Anruf-Button, Karte/Anfahrt
- **Standard – 299 € einmalig:** alles aus Starter, bis zu 4 Bereiche, Bildergalerie, Speisekarte oder Preisliste, WhatsApp-Button für die Kunden des Ladens
- **Upgrade Starter → Standard: 179 €** (steht so auf der Seite; Standard direkt ist günstiger, das sagen wir ehrlich dazu)
- **Pflege – 19 € / Monat (optional):** Änderungen wie Öffnungszeiten, Preise, Fotos, Texte
- Domain kostet extra (ca. 1–15 € pro Jahr) und läuft auf den Namen des Kunden
- Ablauf: Kunde schreibt → kostenlose Vorschau → gefällt sie, wird bezahlt und die Seite geht online; gefällt sie nicht, zahlt er nichts
- Nicht im Angebot: Onlineshops, Buchungssysteme

## Technik

- Reines HTML/CSS/JS, jede Seite eine einzelne Datei. Keine Frameworks, kein Build-Schritt
- Hosting: **GitHub Pages**, live vom Branch `claude/bold-brahmagupta-4h8nrh`
- Domain `salzgitter-webdesign.de` bei IONOS, DNS zeigt auf GitHub Pages. Die Datei `CNAME` niemals löschen oder ändern
- Kontaktformular über FormSubmit (formsubmit.co, kostenlos)
- Jede Seite muss auf dem Handy perfekt aussehen (Mobile First)
- Schnelle Ladezeit: keine externen Schriften oder Bibliotheken, Bilder komprimieren, Grafiken möglichst als CSS/SVG
- Keine Cookies, kein Tracking, keine eingebetteten Google-/Meta-Dienste (sonst wäre ein Cookie-Banner nötig)
- Impressum und Datenschutzerklärung sind Pflicht (Deutschland). Wenn ein neuer externer Dienst dazukommt, die Datenschutzerklärung anpassen

## Aufbau des Repos

| Pfad | Inhalt |
|---|---|
| `index.html` | Firmen-Webseite (Startseite) |
| `impressum.html` | Impressum und Datenschutzerklärung |
| `beispiele/barbershop/`, `beispiele/imbiss/`, `beispiele/baeckerei/` | Beispielseiten für erfundene Läden |
| `zakat-rechner/index.html` | Vermögens- & Zakat-Rechner (mein erstes Projekt, nicht kaputt machen) |
| `webdesign/` | nur Weiterleitungen von alten Links, nicht löschen |
| `CNAME` | Domain für GitHub Pages, nicht anfassen |
| `sitemap.xml`, `robots.txt` | für Google/Bing. Neue öffentliche Seiten in die Sitemap eintragen |
| `og-image.png`, `apple-touch-icon.png` | Vorschaubild für geteilte Links und Handy-Icon. Vorlage: `bilder/vorlagen.html` |
| `instagram/` | Instagram-Posts (`posts.html` = Vorlage, PNGs, `captions.md`) |
| `vertrieb/` | Akquise: `nachrichten.md` (DM-Vorlagen), `flyer.html` (Vorlage) + Flyer/Visitenkarten-PDFs. Die Kunden-Liste (xlsx) gehört NICHT ins Repo (.gitignore) |

- Kontaktdaten, Name, Instagram, Formular-Adresse und Google-Bewertungen stehen im **`CONFIG`-Objekt** ganz oben im Script von `index.html`. Änderungen daran nur dort machen
- Leere Felder im `CONFIG` werden auf der Seite automatisch ausgeblendet

## Ehrlichkeit & Halal

- Keine erfundenen Kundenbewertungen, Kundenzahlen, Referenzen, Logos oder Auszeichnungen
- Google-Bewertungen nur echte, genau so übernommen wie auf Google
- Beispielseiten immer deutlich als „Beispiel“ kennzeichnen, mit `noindex`, erfundene Adressen (Musterstraße)
- Keine Werbung für Alkohol, Glücksspiel oder Zinsprodukte
- Keine Versprechen, die ich nicht halten kann (z. B. „Platz 1 bei Google“)

## Private Daten

- Meine Telefonnummer und Wohnadresse **nicht** auf der Webseite veröffentlichen
- Öffentliche Kontakt-E-Mail ist `kontakt@salzgitter-webdesign.de`
- Das Repo ist öffentlich: alles, was committet wird, kann jeder lesen

## So soll Claude arbeiten

- Antworte auf Deutsch
- Bei größeren Änderungen zuerst einen kurzen Plan zeigen und auf mein OK warten
- Erkläre Änderungen einfach, ich bin kein Profi-Entwickler
- Vor jedem Commit testen: mit Playwright auf Handy- (iPhone, 320 px) und Desktop-Größe, keine JS-Fehler, nichts läuft seitlich aus dem Bildschirm, Links und Formular funktionieren
- Nach jeder fertigen Aufgabe einen Git-Commit mit klarer Beschreibung machen
- Damit Änderungen live gehen, auf `claude/bold-brahmagupta-4h8nrh` pushen. Niemals Force-Push
- Keine kostenpflichtigen Dienste oder Pakete einbauen, ohne mich zu fragen (Budget ist klein)

## Niemals

- Passwörter, API-Keys oder Kundendaten in den Code schreiben oder committen
- Fremde Logos, Bilder oder Texte ohne Erlaubnis verwenden
- Dateien löschen, ohne vorher zu fragen

## Offene Punkte

- Impressum hat zurzeit keine Anschrift (Pflichtangabe!). Sobald eine Geschäftsadresse da ist, in `impressum.html` eintragen
- Kontaktformular muss bei FormSubmit einmal aktiviert werden (Aktivierungs-Mail)
- Google-Unternehmensprofil anlegen, danach Bewertungs-Link im `CONFIG` eintragen
