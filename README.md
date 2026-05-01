# Migration-Sprint 2026

Arbeits- und Dokumentationsrepo fuer die Migration bestehender Sportvereins-Websites in zContent und die zLiga-Hosting- bzw. Vorschau-Struktur.

## Grundauftrag

Bestehende Inhalte, Seitenstrukturen, Vereinsinformationen, externe Links und bereits getroffene Entscheidungen werden strukturiert uebernommen. Die Migration ist keine freie Neugestaltung, sondern eine redaktionell saubere, responsive und CMS-kompatible Uebertragung vorhandener Inhalte.

## Projektregeln

- Keine inhaltlichen Kuerzungen ohne Rueckfrage.
- Keine Umbenennung von Menuepunkten ohne Abstimmung.
- Keine Designaenderungen ohne Freigabe.
- Bestehende Linkziele und CMS-Pfade exakt beachten.
- Platzhalter wie `%CONTENT%`, `%SIDEBAR%` und `%TRAFFIC%` nicht entfernen, wenn sie zur CMS-Logik gehoeren.
- Interne CMS-Links werden projektgenau dokumentiert und verwendet.
- Der Aufwandscheck kann online auf der aktiven Website erfolgen und durch Exportdateien/ZIPs ergaenzt werden.
- Geplanter Standard-Migrationszeitraum fuer News/Berichte/Aktuelles: `06/2025` bis `04/2026`; aeltere Inhalte nur fuer Archiv oder nach Freigabe.

## Arbeitsbereiche

- `docs/`: zentrale Projektregeln, CMS-Konventionen und Vorlagenlogik.
- `checklisten/`: Analyse-, Migrations- und Abnahme-Checklisten.
- `templates/`: allgemeine Vorlage-A- und Vorlage-B-Dokumentation.
- `vereine/`: projektspezifische Dokumentation, Inhalte und Template-Artefakte je Verein.
- `docs/aufwandscheck-schema.md`: Standard fuer Aufwandseinschaetzungen je Verein.
- `docs/leadliste-dunkelbereich.md`: Arbeitsliste fuer potenzielle Vertriebs-/Marketing-Leads.

## Wichtige CMS-Regelquelle

Die Regeln fuer zContent, TinyMCE, Templates, Platzhalter, Formulare, CSS, JS und Asset-Pfade sind in `docs/cms-konventionen.md`, `docs/link-und-asset-regeln.md` und `checklisten/cms-einpflege-checkliste.md` zusammengefasst. Grundlage ist die externe Systemdokumentation `zcontent-cms-dokumentation.md`.
