# Entscheidungen TSV Reinhardtsgrimma

## Vorlagenentscheidung

- Empfehlung im Sprint: eher Variante B.
- Begruendung: Projekt ist begonnen und wirkt in der Zielstruktur ueberschaubarer als grosse Vorlage-A-Mehrspartenprojekte.
- Gleichzeitig ist der Altbestand umfangreicher als eine reine Einsparten-Website; Abteilungen und Fussballbereiche muessen sauber abgebildet werden.

## Design

Aus der Implementierungsdoku:

- Referenzfarben: Gruen / Weiss.
- Primaerfarbe: `#1B7A34`.
- Dunkelgruen: `#0D5C22`.
- Hellgruen: `#4CAF65`.
- Hintergrund / dunkle Flaechen: `#0d0d0d`.

## Technische Entscheidungen

- Template-Set mit separaten Dateien fuer Start, Default, Abteilung, Fussball Maenner, Fussball Jugend, Termine und Kontakt verwenden.
- CSS-Dateien:
  - `/css-file/1771922880-style.css`
  - `/css-file/1771922880-blank.css`
- TinyMCE-Content soll keine eigenen Scripts enthalten.
- System-Platzhalter wie `%CONTENT%`, `%TOPBAR%`, `%NAV_HAUPT%` und `%FOOTER%` beibehalten.

## Offene Abgleichpunkte

- Startseitenpfad aus Sprintkontext vs. Template-Pfad pruefen.
- Kontaktformular-ID `259` vs. `261` pruefen.
- Abteilungsstruktur final mit aktuellem CMS-Stand abgleichen.
- PWA/SEO/CCM19-Status vor Go-Live pruefen.
