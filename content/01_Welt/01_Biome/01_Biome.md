---
type: foldernote
folder: 02_Biome
cssclasses:
  - base no header
---
# Biome

In diesem Ordner werden alle grundlegenden Biome der Welt gepflegt.  
Biome beschreiben wiederkehrende ökologische Räume mit typischen Wetterlagen, Gefahren, Bewohnern, Komponenten und prägenden Merkmalen.

## Zweck

Biome dienen als Grundlage für Regionen und helfen dabei, die Welt konsistent und wiederverwendbar aufzubauen.  
Sie werden zentral gepflegt und später in Regionen referenziert, ohne dass ihre Inhalte doppelt angelegt werden müssen.

## Inhalte eines Biom-Eintrags

- **Kurzbeschreibung**: knappe, sofort lesbare Zusammenfassung.
- **Wetter**: typische klimatische Bedingungen.
- **Gefahren**: natürliche oder situative Risiken.
- **Bewohner**: typische Fauna, Vegetation oder andere Präsenzformen.
- **Komponenten**: dort auffindbare Jagd-, Fisch-, Material- und Kräuterkunde-Elemente.
- **Merkmale**: prägende sensorische, emotionale oder physische Eindrücke.
- **Begehbarkeit**: wie leicht oder schwer das Biom passierbar ist.
- **Sicht**: wie offen oder eingeschränkt die Wahrnehmung dort ist.

## Pflegehinweise

- Neue Biome immer als eigene Notiz anlegen.
- Die Struktur möglichst einheitlich halten.
- Biome nicht mit regionsspezifischen Sonderfällen überladen.
- Konkrete Spielrollen und Szenennutzung gehören eher in die jeweilige Region.
- Mehrere Biome können später in einer Region kombiniert werden.

## Navigation
```base
filters:
  and:
    - file.folder.startsWith("01_Welt/01_Biome")
views:
  - type: table
    name: Table
    filters:
      and:
        - file.name != "01_Biome"
    order:
      - file.name
      - beschreibung_kurz
      - bewohner
      - gefahren
      - kategorie
      - komponenten

```


```base
filters:
  and:
    - file.inFolder("01_Welt/01_Biome")
    - type == "biom"
formulas:
  anzahl_jagen: Jagen.length
  anzahl_fischen: Fischen.length
  anzahl_materialien: Materialien.length
  anzahl_kraeuter: Kräuter.length
  anzahl_gesamt: formula.anzahl_jagen+formula.anzahl_fischen+Formula.anzahl_materialien+Formula.anzahl_kraeuter
views:
  - type: table
    name: Komponenten je Biom
    order:
      - name
      - formula.anzahl_jagen
      - formula.anzahl_fischen
      - formula.anzahl_kraeuter
      - formula.anzahl_materialien
      - formula.anzahl_gesamt
    sort:
      - property: formula.anzahl_gesamt
        direction: ASC
    columns:
      - note.name as Biom
      - formula.anzahl_jagen as Jagen
      - formula.anzahl_fischen as Fischen
      - formula.anzahl_materialien as Materialien
      - formula.anzahl_kraeuter as Kräuter
      - formula.anzahl_gesamt as Gesamt
    columnSize:
      note.name: 153
      formula.anzahl_jagen: 113
      formula.anzahl_fischen: 141

```