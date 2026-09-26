# Tablefy Dashboard

Custom Code der Webflow-Dashboard-Seite auf tablefy.app. Export vom 26.09.2026.

## Dateien

- `original__*.html`: 41 HTML-Embeds und die vier unveränderten Head-/Footer-Blöcke von Seite und Projekt.
- `script__*.js`: 35 separat extrahierte JavaScript-Blöcke.
- `style__*.css`: 22 separat extrahierte CSS-Blöcke.
- `manifest.json`: Zuordnung zu Webflow-Elementen, ursprüngliche Abfragereihenfolge und SHA-256-Prüfsummen.
- `external-dependencies.json`: externe Script-/Stylesheet-Links mit ihren Attributen.
- `syntax-checks.json`: alle 35 JavaScript-Blöcke bestehen `node --check`.

## Nutzung

Die HTML-Dateien sind die maßgeblichen Originalquellen. JS und CSS wurden daraus unverändert extrahiert und sind alternative Bearbeitungsdateien; nicht zusätzlich zu den Originalen einbinden.

Dies ist eine Übernahme des vorhandenen Codes zur Versionsverwaltung. Webflow lädt weiterhin seine bisherigen Einbindungen. Die Dateien sind kein automatisch ladbares Gesamtbundle. Vor einer Umstellung müssen die tatsächliche Ausführungsreihenfolge, DOM-Positionen und Attribute wie defer, async und integrity erhalten und im Browser geprüft werden. Die Embed-Nummern bilden die API-Abfragereihenfolge ab und garantieren keine Laufzeitreihenfolge.

Externe Dateien sind als Referenzen erfasst; ihre Inhalte sind nicht kopiert. Visuelle Webflow-Styles, Interactions und Seitenmarkup außerhalb der Embeds gehören nicht zu diesem Export. Die getrennten registrierten Script-Endpunkte lieferten HTTP 404; die Antworten stehen im Manifest.

Der öffentliche Supabase-Anon-Key bleibt wie im Frontend enthalten. Keine Datenbankdaten wurden exportiert. Es erfolgte eine Syntaxprüfung, kein Laufzeittest.
