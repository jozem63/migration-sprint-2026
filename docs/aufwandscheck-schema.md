# Aufwandscheck-Schema

## Zweck

Einheitliches Schema fuer den schnellen Aufwandscheck je Verein. Der Check kann online auf der aktiven Website erfolgen und wird, falls vorhanden, mit Exportdateien/ZIPs abgeglichen.

## Grundregel

- Online-Check ist erlaubt, solange die alte Website erreichbar ist.
- Export/ZIP ist Zusatzquelle und kann die gesamte Website enthalten.
- Geplanter Standard-Migrationszeitraum fuer News/Berichte/Aktuelles: `06/2025` bis `04/2026`.
- Dauerhafte Inhalte wie Verein, Vorstand, Kontakt, Impressum, Datenschutz, Satzung, Downloads, Formulare, Abteilungen und Sponsoren werden unabhaengig vom Datum geprueft.
- Aeltere Inhalte nur fuer Archiv oder nach Freigabe uebernehmen.

## Bewertung

| Stufe | Bedeutung | Typischer Umfang |
|---|---|---|
| klein | kompakte Website, wenige Seiten, wenig Archiv | Einspartenverein oder kleine Vereinsseite |
| mittel | mehrere Bereiche, normale Downloads, ueberschaubare News | Mehrspartenverein mit klarer Struktur |
| gross | viele Abteilungen/Mannschaften, viele Medien, tiefe Archive | TSV/Fussballverein mit Mannschaftsstruktur |
| Sonderfall | fehlender Export, unklare Rechte, sehr grosse Datenmenge, Angebot/ Auftrag offen | Vor Umsetzung klaeren |

## Vorlage fuer `aufwandscheck.md`

```md
# Aufwandscheck [Verein]

## Kurzstatus

| Punkt | Ergebnis |
|---|---|
| Domain |  |
| Staging |  |
| Projektstatus |  |
| Go-Live / Realisierungsstand |  |
| Vorlage |  |
| Online-Check | offen / erledigt |
| Export / ZIP | vorhanden / fehlt / unklar |
| Migrationszeitraum | 06/2025 bis 04/2026 |
| Aufwand | klein / mittel / gross / Sonderfall |

## Quellen

- Aktive Website:
- Export / ZIP:
- Projektdateien:
- CMS / Staging:

## Online-Check

- [ ] Website erreichbar
- [ ] Footer/Technikhinweis geprueft
- [ ] Hauptnavigation aufgenommen
- [ ] Abteilungen / Mannschaften aufgenommen
- [ ] News / Aktuelles im Zeitraum `06/2025` bis `04/2026` geprueft
- [ ] Downloads / Formulare geprueft
- [ ] Impressum / Datenschutz geprueft
- [ ] Externe Profile / Widgets geprueft

## Export-Check

- [ ] ZIP vorhanden
- [ ] Seitenzahl / HTML-Dateien gezaehlt
- [ ] Medienzahl gezaehlt
- [ ] PDF-/Downloadzahl gezaehlt
- [ ] SQL-Dump vorhanden
- [ ] Export gegen Online-Struktur abgeglichen

## Pflichtseiten

- Startseite:
- Verein:
- Vorstand / Ansprechpartner:
- Kontakt:
- Impressum:
- Datenschutz:
- Downloads:
- Sponsoren / Partner:

## Abteilungen / Mannschaften

- 

## Relevante Inhalte 06/2025 bis 04/2026

- News / Berichte:
- Termine:
- Mannschaftsberichte:
- Sonstiges:

## Dauerhafte Inhalte

- Downloads / Formulare:
- Satzung / Ordnungen:
- Kontakt / Vorstand:
- Abteilungsseiten:
- Sponsoren:

## Risiken / offene Punkte

- 

## Aufwandseinschaetzung

**Stufe:** klein / mittel / gross / Sonderfall

**Begruendung:**

- 

## Naechster Schritt

- 
```

## Priorisierte Anwendung

1. SG Geising: Auftrag fehlt, Nachfassen.
2. HD Tennis Academy: Angebot erstellen.
3. SV Hellern: kein Export/Zugang dokumentiert, Online-Check und Exportbedarf.
4. VfL Wildenfels: kein Altseitenexport im ZIP, Online-Check und Exportbedarf.
5. Grosse Exporte: TSV Meine, SC Gaissach, Teltower FV 1913.
