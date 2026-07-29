---
type: foldernote
folder: 03_Merkmale
---
# Merkmale

In diesem Ordner werden alle **Merkmale** für Komponenten gepflegt.  
Merkmale beschreiben, wie etwas wahrgenommen wird, welche Stimmung es auslöst oder welche körperliche oder stoffliche Wirkung es hat. Bei der Verwendung der Komponente dienen die Merkmale als Bezugspunkte.

## Kategorien

- **Sensorisch**: Beschreibung von Geschmack, Geruch, Textur, Klang oder allgemeinem Eindruck.
- **Emotional**: Beschreibung der Stimmung oder Reaktion, die beim Konsum oder Gebrauch ausgelöst wird.
- **Physisch / Physiologisch**: Beschreibung direkter körperlicher Wirkungen wie Wärme, Energie, Beruhigung oder Regeneration.
- **Materialeigenschaften**: Beschreibung physischer Eigenschaften eines Stoffes, etwa Härte, Stabilität, Resistenz oder Leitfähigkeit.

## Pflegehinweise

- Neue Merkmale werden als eigene Notiz im Ordner `03_Merkmale` angelegt.
- Die Frontmatter-Felder des Merkmal-Templates sollen konsistent verwendet werden.
- Merkmale werden zuerst Komponenten zugeordnet, später können sie auch für Biome, Regionen und andere Entitäten genutzt werden.

## Tabellarische Übersicht
```base
filters:
  and:
    - file.folder.startsWith("01_Welt/03_Merkmale")
views:
  - type: table
    name: Table
    filters:
      and:
        - file.name != "03_Merkmale"
    order:
      - kategorie
      - file.name
      - narrative_wirkung
      - verwendet_in
    sort:
      - property: verwendet_in
        direction: ASC
      - property: kategorie
        direction: DESC

```

