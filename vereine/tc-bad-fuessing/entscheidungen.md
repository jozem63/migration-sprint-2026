# Entscheidungen TC Bad Fuessing

## Vorlagenentscheidung

- Empfehlung im Sprint: Variante B.
- Begruendung: Einspartenverein Tennis mit kompakter Grundstruktur.
- Die Projektunterlagen bestaetigen einen schlanken Migrationsprozess mit Coming-soon-Seite und Generator-Workflow.

## Design

- Primaerfarbe: `#BFCE00` Tennisball-Gruen.
- Sekundaerfarbe: `#1E3D7A` Vereinsblau.
- Coming-soon-Design: dunkler Navy-Hintergrund, Tennisplatz-Textur, Barlow / Barlow Condensed.
- Logo und Favicon aus dem Bestand verwenden.

## Technische Besonderheiten

- Umlaut-Domain: Produktivdomain technisch als ACE-Domain behandeln.
- Python-Generatoren vorhanden:
  - `DOC/tcbf_master_generator_v2.py`
  - `DOC/tcbf_master_generator_v3.py`
  - `Claud-Projekt/svh_master_generator.py` als fremde/vergleichende Generatorbasis
- `v3` ist als neuerer TC-Bad-Fuessing-Stand zu behandeln.

## Sicherheit / Datenschutz

Personenbezogene Kontaktdaten aus Erstkontaktdateien werden nicht ins GitHub-Repo uebernommen. Zugangsdaten, AuthCodes und Vertragsdaten gehoeren nicht in die Projektdokumentation.
