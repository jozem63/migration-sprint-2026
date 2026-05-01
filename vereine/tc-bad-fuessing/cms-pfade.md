# CMS-Pfade TC Bad Fuessing

## Grunddaten

- CMS-Lizenz: `1775552926`
- Staging: `https://tc-bad-fuessing.zliga.de`
- Produktiv-Domain: `tc-bad-fuessing.de`
- ACE-Domain: `xn--tc-bad-fssing-3ob.de`
- CMS-Login: `https://kundenlogin.id-zemke.de/`

## Bekannte Staging-Bildpfade

Aus Erstkontakt und Projektdatei:

| Datei | Staging-Pfad |
|---|---|
| Logo mit weissem Hintergrund | `https://tc-bad-fuessing.zliga.de/bilder/1775552926/1775552926-1775559619-tc_bad_fuessen_logo_bg_white.jpg` |
| Logo 1:1 | `https://tc-bad-fuessing.zliga.de/bilder/1775552926/1775552926-1775559669-tc_bad_fuessen_logo_1_1.png` |
| Favicon | `https://tc-bad-fuessing.zliga.de/bilder/1775552926/1775552926-1775559697-favicon.png` |

## Umlaut-Domain-Regel

| Zweck | Schreibweise |
|---|---|
| Anzeige im Text | `tc-bad-fuessing.de` bzw. lesbar mit Umlaut nach Abstimmung |
| href / canonical / technische URLs | `xn--tc-bad-fssing-3ob.de` |

## Backend-Dienste

Beim URL-Migrationsscript nicht auf Produktivdomain ersetzen:

- `ezcounter.php`
- `lastupdate.php`
- `ezsiterss.php`
- `ezcalendar.php`
- `ezcalendar_short.php`
- `ezsite.php`
