# CMS-Einpflege-Checkliste

## Projektbasis

- [ ] Projekt-ID / CMS-Lizenz dokumentiert
- [ ] Staging-URL dokumentiert
- [ ] Produktiv-Domain dokumentiert
- [ ] Startseitenpfad dokumentiert
- [ ] Template-Namen dokumentiert

## Templates

- [ ] Standardtemplate fuer Inhaltsseiten festgelegt
- [ ] Sondertemplate fuer Kontaktformular festgelegt
- [ ] News-/Mannschafts-/Sidebar-Templates bei Bedarf festgelegt
- [ ] `%CONTENT%` auf Inhaltsseiten vorhanden
- [ ] `%CANONIAL-URL%` exakt so geschrieben
- [ ] `%APP%` innerhalb von `<body>`
- [ ] Keine Platzhalter-Tokens in HTML-Kommentaren
- [ ] Open-Graph-Tokens im `<head>` geprueft
- [ ] Alle Bilder mit `alt`-Attribut

## Platzhalter

- [ ] `%TOPMENU%` als zentraler Navigationsplatzhalter angelegt oder Projektabweichung dokumentiert
- [ ] `%FOOTER%` als zentraler Footerplatzhalter angelegt oder Projektabweichung dokumentiert
- [ ] `%SIDEBAR%` bei Sidebar-Templates angelegt
- [ ] `%SEITENTITEL%` mit Bedingungen je Seiten-Nummer oder Fallback angelegt
- [ ] Widget-Platzhalter fuer FuPa/fussball.de/Staige.tv angelegt
- [ ] Fuer alle bedingten Platzhalter ein Fallback `Ohne Bedingung` vorhanden

## TinyMCE-Editor

- [ ] Keine `<script>`-Tags im Editor
- [ ] Keine `<style>`-Tags im Editor
- [ ] Keine Inline-Styles `style="..."` im Editor
- [ ] Nur Klassen verwenden, die in `blank.css` vorhanden sind
- [ ] Keine Widget-Codes im Editor
- [ ] Keine eigenen `<form>`-Tags im Editor

## CSS und JS

- [ ] Projekt-CSS ueber `/css-file/[ID]-dateiname.css` eingebunden
- [ ] `blank.css` aus `blank-muster.css` abgeleitet
- [ ] Systemklassen in `blank.css` nicht umbenannt
- [ ] Projekt-JS als externe Datei im Bilderpfad eingebunden
- [ ] Kein Inline-JavaScript in Editorinhalten
- [ ] Bootstrap-Bundle nur einmal eingebunden

## Formulare

- [ ] Formular-Typ `Webseiten-Template` verwendet
- [ ] Formularwebseite mit `index-contact.html` verbunden
- [ ] Im Editor nur Felder, Labels und Textareas
- [ ] E-Mail-Feldname exakt `EMail`
- [ ] reCAPTCHA-Script im Template, nicht im Editor
- [ ] Erfolgsseite / Danke-Seite gesetzt
- [ ] Formularversand getestet

## Medien und Links

- [ ] Bildpfade nach CMS-Schema geprueft
- [ ] CSS-Pfade nach CMS-Schema geprueft
- [ ] JS-Pfade nach CMS-Schema geprueft
- [ ] Favicon-Pfade geprueft
- [ ] Interne CMS-Links exakt uebernommen
- [ ] Externe Links mit Ziel und Zweck dokumentiert

## Abschluss

- [ ] Seite nach Template-Upload im Browser geprueft
- [ ] Navigation funktioniert auf Desktop und Mobil
- [ ] Carousel / Slider hat Bootstrap-konforme Buttons
- [ ] Encoding / Umlaute geprueft
- [ ] Keine sichtbaren Platzhaltertexte
- [ ] Keine sichtbaren Kommentarreste
- [ ] Editor-Inhalte speichern korrekt
