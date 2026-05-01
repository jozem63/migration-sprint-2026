# CMS-Konventionen

Grundlage: zContent CMS Systemdokumentation, Stand April 2026. Diese Regeln gelten fuer alle Migrationen, sofern projektbezogen nichts anderes freigegeben ist.

## Systemprinzip

- zContent ist ein eznews-basiertes CMS mit serverseitigem Placeholder-Templating.
- Jede Seite verwendet eine Template-Datei wie `index.html`, `index_default.html`, `index_news.html` oder `index-contact.html`.
- Inhalte werden im TinyMCE-Editor gepflegt und ueber `%CONTENT%` eingebunden.
- Design, Layout, Navigation, Footer, CSS und JavaScript gehoeren ins Template, in CSS-Dateien, JS-Dateien oder CMS-Platzhalter, nicht in den Editor.
- Fuer Sonderfunktionen wie Kontaktformulare, News oder Mannschaftsseiten eigene Templates verwenden.

## Template-Regeln

- `%CONTENT%` ist Pflicht auf Inhaltsseiten.
- Startseiten koennen als `index.html` fest kodiert sein und muessen nicht zwingend `%CONTENT%` nutzen.
- Das Standardtemplate fuer Inhaltsseiten soll als Standard im CMS markiert werden.
- Sonderseiten wie Kontaktformular, News oder Mannschaftsseiten muessen explizit dem passenden Template zugewiesen werden.
- Keine `%PLATZHALTER%`-Tokens in HTML-Kommentaren verwenden. zContent ersetzt Tokens auch innerhalb von Kommentaren; dadurch kann sichtbarer Fehlertext entstehen.
- `%APP%` muss innerhalb von `<body>` stehen.
- `%CANONIAL-URL%` exakt so schreiben. Der Tippfehler ist systembedingt und darf nicht korrigiert werden.
- Alle Bilder mit `alt`-Attribut versehen.
- Sonderzeichen in kritischen Template-Texten, Buttons und Carousel-Controls als HTML-Entities schreiben.

## Platzhalter

Wichtige System- und Projektplatzhalter:

- `%CONTENT%`
- `%SEITENTITEL%`
- `%NEWSSTART%`
- `%FB-TITEL%`
- `%FB-DESCRIPTION%`
- `%FB-BILD%`
- `%CANONIAL-URL%`
- `%APP%`
- `%TOPMENU%`
- `%FOOTER%`
- `%SIDEBAR%`
- `%TRAFFIC%`
- `%WIDGET-ID-X%`

Diese Platzhalter duerfen nicht entfernt werden, wenn sie in der jeweiligen Vorlage benoetigt werden.

## Benutzerdefinierte Platzhalter

- Navigation und Footer bevorzugt zentral als CMS-Platzhalter vom Typ `Quelltext` pflegen.
- `%TOPMENU%` fuer Navigation verwenden, wenn mehrere Templates dieselbe Navigation nutzen.
- `%FOOTER%` fuer den Footer verwenden, wenn projektbezogen vorgesehen.
- `%SIDEBAR%` fuer seitliche Navigation oder Zusatzboxen verwenden.
- `%SEITENTITEL%` kann ueber Bedingungen je Seiten-Nummer gepflegt werden.
- Fuer bedingte Platzhalter immer einen Fallback `Ohne Bedingung` anlegen.

## Widget-Regel

- Externe Widgets wie FuPa, fussball.de oder Staige.tv gehoeren nicht in den TinyMCE-Editor.
- Widget-Code mit HTML und Script als CMS-Platzhalter vom Typ `Quelltext` anlegen.
- Im Template nur den Widget-Platzhalter einbinden, z. B. `%WIDGET-ID-MANNSCHAFT1%`.
- Der TinyMCE-Editor entfernt `<script>`- und `<style>`-Tags, daher wuerden Widgets im Editor zerstoert.

## TinyMCE-Editor

Im Editor erlaubt:

- Reines semantisches HTML
- Texte, Listen, Tabellen, Links und Bilder
- `class="..."`, wenn die Klasse in `blank.css` vorhanden ist
- Iframes ohne eigenes JavaScript, z. B. YouTube oder OpenStreetMap, falls projektbezogen freigegeben

Im Editor verboten:

- `<script>`-Tags
- `<style>`-Tags
- Inline-Styles wie `style="..."`
- Widget-Code mit Script
- Eigene `<form>`-Tags
- reCAPTCHA-Scripts oder Formular-Submit-Buttons

## CSS-Regeln

- Layout- und Template-Klassen gehoeren in die Projekt-CSS, z. B. `style.css`.
- Editor-Klassen fuer TinyMCE gehoeren in `blank.css`.
- `blank.css` muss auf der systemseitigen `blank-muster.css` basieren.
- Systemklassen duerfen nicht umbenannt werden.
- Projektfarben, Fonts und Werte der Systemklassen duerfen angepasst werden.
- CSS-Dateien liegen im CMS unter `/css-file/[PROJEKT-ID]-dateiname.css`.
- Keine zusaetzlichen CSS-Dateien einbauen, wenn sie nicht projektbezogen abgestimmt sind.

Pflichtklassen aus `blank-muster.css`:

- `.normal`
- `.text`
- `.pokal`
- `.ueberschrift`
- `.ueberschrift2`
- `.ueberschrift3`
- `.link`
- `.link_aktiv`
- `.auswahl`
- `.bemerkung`

## JavaScript-Regeln

- Kein JavaScript im TinyMCE-Editor.
- Kein Inline-JavaScript in Templates, wenn es vermeidbar ist.
- Projekt-JavaScript als externe Datei ueber die Dateiverwaltung hochladen.
- JS-Dateien liegen technisch im Bilderpfad: `/bilder/[PROJEKT-ID]-[DATEI-ID]-dateiname.js`.
- Bootstrap-Bundle und Projekt-JS am Ende von `<body>` einbinden.
- Lightbox, ScrollUp, Click-to-Play oder Akkordeons immer ueber externe JS-Dateien loesen.

## Formular-Regeln

- Kontaktformulare laufen als Formular-Typ `Webseiten-Template`.
- Das CMS erzeugt das `<form>`-Tag, den Submit-Button, Versand und reCAPTCHA-Validierung.
- Im TinyMCE-Editor stehen nur Formularfelder: `label`, `input`, `textarea`, `select`.
- Kein eigenes `<form>`-Tag im Editor.
- Kein Button und kein reCAPTCHA-Script im Editor.
- reCAPTCHA-Script gehoert ins Template `index-contact.html`.
- E-Mail-Feldname exakt `EMail` schreiben.
- Formularseiten muessen das passende Kontakt-Template verwenden.

## Medien- und Dateipfade

- Bilder: `/bilder/[PROJEKT-ID]/[PROJEKT-ID]-[DATEI-ID]-dateiname.ext`
- CSS: `/css-file/[PROJEKT-ID]-dateiname.css`
- JS: `/bilder/[PROJEKT-ID]-[DATEI-ID]-dateiname.js`
- Favicons PNG: `/bilder/[PROJEKT-ID]/[PROJEKT-ID]-[DATEI-ID]-favicon-*.png`
- Favicon ICO: `/bilder/[PROJEKT-ID]-[DATEI-ID]-favicon.ico`

## Encoding und Sonderzeichen

- Bei Buttons, Carousel-Controls und kritischen Template-Texten HTML-Entities verwenden.
- `&copy;` immer mit Semikolon schreiben.
- Bekannte Entities: `&auml;`, `&ouml;`, `&uuml;`, `&Auml;`, `&Ouml;`, `&Uuml;`, `&szlig;`, `&copy;`, `&ndash;`, `&rarr;`.
- Wenn ein Editor-Inhalt ohne Fehlermeldung nicht speichert, auf Spam-Filter-Woerter pruefen. Bestaetigtes Problemwort: `sleep`.

## HTML-Ausgaben

- Bootstrap 5.3.x verwenden, wenn die bestehende Vorlage darauf basiert.
- Vollstaendig responsiv aufbauen.
- Semantisch sauberes HTML verwenden.
- Bestehende Klassen und Stylesheets nutzen.
- Interne CMS-Links exakt uebernehmen.
- Keine erklaerenden Projektkommentare mit Platzhalter-Tokens im HTML lassen.

## BSV 1924 Scripts und Styles

- Projekt-CSS: `/css-file/1773736856-style.css`
- Lightbox-Script: `/bilder/1773736856-1776864363-script.js`
- Lightbox-Script in relevanten Templates einbinden.
- Ausnahme: `index-contact.html` ohne Lightbox-Script.
