# Soziologische Grundlagen

Interaktives Skript zur Lehrveranstaltung „1.10.1 Soziologische Grundlagen“ von Prof. Dr. Mehmet Kart, Soziale Arbeit (B. A.), OTH Regensburg (SoSe 2026, Gruppe Freitag).

## Was wo liegt

```
welcome.qmd              Willkommensseite
index.qmd                Seminarüberblick (Startseite der Webseite)
grundlagen/              Grundbegriffe zum Aufklappen
sitzungen/               Sitzungen nach dem Seminarplan (bisher 1, 2, 3 und 7)
03-lernspiele.qmd        Lernspiele (Memory, Aussagen zuordnen)
04-lernkontrolle.qmd     Lernkontrolle
interactions/            die drei Lernspiele als HTML-Dateien
images/                  Abbildungen
fonts/                   Schrift Outfit (OTH), lokal eingebunden
include/                 Technik: Höhe der Lernspiele, aufklappbare Theorien
_quarto.yml              Einstellungen (Titel, Navigation links, Fußzeile)
styles.scss              Layout im OTH-Design
apa.csl                  Zitierstil
docs/                    fertige Webseite (wird automatisch erzeugt, nicht von Hand ändern)
```

Welche Seiten gebaut werden, steht in `_quarto.yml` unter `render:`.

## Neue Sitzung hinzufügen

Neue `.qmd`-Datei unter `sitzungen/` anlegen (z. B. `sitzungen/04-marx-kritische-theorie.qmd`), in `_quarto.yml` unter `sidebar: contents:` eintragen und in `index.qmd` den Sitzungstitel verlinken.

## Lernspiele ändern

In jeder Datei unter `interactions/` steht oben ein Block `DATEN`. Nur dort Begriffe, Aussagen oder Fragen ändern; der Rest ist Technik.

## Webseite aktualisieren

1. `.qmd`-Datei in RStudio bearbeiten und speichern.
2. Im Reiter *Terminal*: `quarto render`
3. In GitHub Desktop: kurze Notiz eintragen, **Commit to main**, dann **Push origin**.

Nach ein bis zwei Minuten ist die Webseite aktualisiert (im Browser mit Strg+F5 neu laden).
