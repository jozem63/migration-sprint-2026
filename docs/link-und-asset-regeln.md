# Link- und Asset-Regeln

## Interne Links

- Interne CMS-Links exakt aus zContent uebernehmen.
- Keine CMS-Pfade eigenstaendig umbenennen.
- Bekannte Pfade in `cms-pfade.md` je Verein dokumentieren.
- Bei Navigationen bevorzugt den zentralen Platzhalter `%TOPMENU%` verwenden.
- Neue Menuepunkte erst nach Seitenanlage im CMS und Pfadpruefung eintragen.

## Externe Links

- Externe Vereinsprofile wie fussball.de, FuPa, Fanshop oder Social Media dokumentieren.
- Ziel-URLs nicht kuerzen oder ersetzen.
- Externe Links mit `target="_blank"` und `rel="noopener"` verwenden, wenn sie in neuem Tab oeffnen.
- Widget-Links nicht in TinyMCE einkleben, wenn Script-Code erforderlich ist; dafuer CMS-Platzhalter vom Typ `Quelltext` nutzen.

## Asset-Pfade

- Bilder: `/bilder/[PROJEKT-ID]/[PROJEKT-ID]-[DATEI-ID]-dateiname.ext`
- CSS: `/css-file/[PROJEKT-ID]-dateiname.css`
- JS: `/bilder/[PROJEKT-ID]-[DATEI-ID]-dateiname.js`
- Favicons PNG: `/bilder/[PROJEKT-ID]/[PROJEKT-ID]-[DATEI-ID]-favicon-*.png`
- Favicon ICO: `/bilder/[PROJEKT-ID]-[DATEI-ID]-favicon.ico`

## Medienuebernahme

- Vereinslogo unverfaelscht verwenden.
- Bilder seitenbezogen aus Export oder aktiver Website pruefen.
- Altmedien nicht massenhaft ungeprueft in neue Inhalte einbauen.
- Downloads/Formulare/Satzung/Datenschutz/Impressum auf Aktualitaet pruefen.
- Projekt-, Angebots-, Muster- und Agenturdateien nicht als Website-Downloads uebernehmen.

## TinyMCE und Assets

- Im TinyMCE-Editor keine Inline-Styles verwenden.
- Bildgestaltung ueber Klassen aus `blank.css` loesen.
- Iframes nur nach Projektfreigabe und ohne eigenes JavaScript verwenden.
- Widget-Code mit Script immer als CMS-Platzhalter anlegen.

## Encoding

- Kritische Sonderzeichen in Template-Texten als HTML-Entities schreiben.
- Besonders Button-, Carousel- und Navigationstexte nach Upload im Browser pruefen.
- `&copy;` immer mit Semikolon verwenden.
