# Vertrieb: Dunkelbereich sportverein-homepage.de

## Ziel

Ermitteln, welche Vereine nach der erforderlichen Abschaltung bzw. Migration von `sportverein-homepage.de` potenziell noch nicht aktiv auf id-zemke.de zugekommen sind.

## Grundannahme

Viele betroffene Websites sind noch online und zeigen im Footer oder Impressum Hinweise wie:

- `Powered by sportverein-homepage.de`
- `Homepage erstellt von sportverein-homepage.de`
- Links zu `sportverein-homepage.de`

Diese oeffentlichen Hinweise koennen fuer eine Recherche genutzt werden.

## Recherche-Regeln

- Nur oeffentlich sichtbare Vereins- und Website-Daten erfassen.
- Keine privaten Ansprechpartnerdaten, Telefonnummern, Bankdaten oder personenbezogene Details ins Repo uebernehmen.
- Treffer immer gegen bestehende Projektliste abgleichen.
- Bereits bekannte oder laufende Projekte markieren, nicht doppelt ansprechen.
- Vor einer Marketingaktion rechtlich sauber pruefen, welche Kontaktform erlaubt ist.
- Keine Massenmail ohne Einwilligung. Besser: individuelle Ansprache ueber oeffentliche Vereinskontaktwege, Telefon/Brief oder Kontaktformular nach rechtlicher Pruefung.

## Suchmuster

Geeignete Suchanfragen:

```text
"Powered by sportverein-homepage.de"
"Homepage erstellt von" "sportverein-homepage.de"
site:sportverein-homepage.de "Referenzen"
site:*.de "Powered by sportverein-homepage.de" Verein
```

## Trefferkategorien

| Kategorie | Bedeutung | Aktion |
|---|---|---|
| Bekannt / im Sprint | Verein ist bereits im Projekt | nicht als Kaltkontakt behandeln |
| Potenzieller Dunkelbereich | Website zeigt sportverein-homepage.de, nicht in Projektliste | fuer Vertriebspruefung vormerken |
| Nicht passend | kein Sportverein oder bereits migriert | nicht weiter verfolgen |
| Unklar | Treffer braucht manuelle Pruefung | online pruefen |

## Erste oeffentliche Kandidaten

Diese Liste ist ein erster Startpunkt aus oeffentlicher Websuche, keine abgeschlossene Leadliste. Jeder Treffer muss vor Ansprache manuell verifiziert und gegen bestehende Projekte abgeglichen werden.

| Verein / Organisation | Domain | Hinweis | Status |
|---|---|---|---|
| SG Parr Medelsheim | sgparr.de | Footer `Powered by sportverein-homepage.de` | potenzieller Dunkelbereich |
| Siedlung Grolland I | grollandeins.de | Footer `Powered by sportverein-homepage.de`; keine klassische Sportvereinsmigration | pruefen / ggf. nicht passend |
| DC Bayernstueberl | dcbayernstberl.sportverein-homepage.de | Subdomain bei sportverein-homepage.de | potenzieller Dunkelbereich |
| Park links der Weser e.V. | parklinksderweser.de | Footer / Erstellerhinweis sportverein-homepage.de | pruefen / ggf. nicht Sportverein |
| Sportverein Borna e.V. | svborna.de | Footer `Powered by sportverein-homepage.de` | potenzieller Dunkelbereich |
| Sport+Akrobatik 1999 e.V. Mainz-Laubenheim | sav-mainz.de | Footer `Powered by sportverein-homepage.de` | potenzieller Dunkelbereich |
| SV Voerden von 1923 e.V. | svvoerden.de | Footer `Powered by sportverein-homepage.de` | potenzieller Dunkelbereich |
| SV 1913 Niedernhausen e.V. | svniedernhausen.de | Footer / Erstellerhinweis sportverein-homepage.de | potenzieller Dunkelbereich |
| SV Hohentengen | offen | Referenz auf sportverein-homepage.de | recherchieren |

## Bereits bekannte Treffer aus Suche

Diese Treffer sind nicht als Dunkelbereich zu behandeln, weil sie bereits im Sprint sind:

- SC Gaissach
- Teltower FV 1913

## Empfohlener Workflow

1. Oeffentliche Trefferliste erstellen.
2. Gegen `sprint-status.md` abgleichen.
3. Pro Kandidat Kurzcheck:
   - Website erreichbar?
   - Footer/Impressum mit sportverein-homepage.de?
   - Sportverein oder andere Organisation?
   - Aktuelle Inhalte vorhanden?
   - Migrationsbedarf wahrscheinlich?
4. Kandidaten priorisieren:
   - A: aktive Sportvereine mit eigener Domain
   - B: aktive Vereine/Organisationen mit eigener Domain
   - C: Subdomain bei sportverein-homepage.de
   - D: unklar / manuell pruefen
5. Erst danach individuelle Vertriebsaktion vorbereiten.

## Vertriebsnotiz

Die Ansprache sollte nicht wie eine automatisierte Kaltmail wirken. Inhaltlich sinnvoll:

- konkreter Hinweis auf die erkennbare technische Abhaengigkeit von sportverein-homepage.de
- kurzer Hinweis auf laufende Migrationen anderer Vereine
- Angebot eines unverbindlichen Kurzchecks
- keine Panikkommunikation, sondern klare Frist- und Loesungsorientierung
