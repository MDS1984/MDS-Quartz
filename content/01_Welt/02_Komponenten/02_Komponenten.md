---
type: foldernote
folder: 02_Komponenten
---
# Komponenten

In diesem Ordner werden alle **Komponenten** gepflegt, aus denen später Tränke, Rezepte, Rituale oder Ausrüstungseigenschaften zusammengesetzt werden können. Komponenten sind die „Bausteine“ der Spielwelt: Kräuter, Materialien, seltene Essenzen, besondere Kreaturenbestandteile usw.

## Kategorien

- **Jagen**: Groß-, Kleinwild, Vögel und Amphibien mit zugeordneten sensorischen, emotionalen und physisch/Physiologischen Merkmalen
	- Besitzt 3 Merkmale: jeweils 1x `Sensorisch`, 1x `Emotional`, 1x `Physchich/Physiologisch`. 1 Merkmal ist davon beim ersten Fund vorausgefüllt.
- **Fischen**: Umfasst Meeres- und Flussfische, sowie Krebse, Krabben und ähnliches.
	- Besitzt 3 Merkmale: jeweils 1x `Sensorisch`, 1x `Emotional`, 1x `Physchich/Physiologisch`. 1 Merkmal ist davon beim ersten Fund vorausgefüllt.
- **Kräuterkunde**: Pflanzen, Pilze und alchemistische Kräuter mit sensorischen und narrativen Wirkungen.
	- Besitzt 2 Merkmale: 1x `Sensorisch`, 1x der Name 
- **Materialkunde**: Metalle, Hölzer, Glas, Stein, Knochen und ähnliche Stoffe mit besonderen Materialeigenschaften.
	- Besitzt 1-3 Merkmale: `Materialeigenschaften`

Jede Komponente wird als eigene Notiz mit `type: komponente` angelegt und enthält:

- `kategorie` (z.B. `kraeuterkunde`, `materialkunde`)
- `biome` (Vorkommen)
- `merkmale` (Verweise auf Merkmals-Notizen)
- eine kurze Beschreibung und Inspirationsideen für Wirkungen.

## Pflegehinweise

- Neue Komponenten werden als eigene Notiz im Ordner `02_Komponenten` bzw. in einem passenden Unterordner angelegt.
- Die Frontmatter-Felder sollen konsistent verwendet werden, damit Filter und Auswertungen funktionieren.
- Die zentrale Übersicht und Pflege der Komponenten erfolgt über diese Seite und ggf. zusätzliche Index-Seiten (z.B. nach Typ oder Merkmal).
- Komponenten verweisen auf Merkmale (z.B. sensorisch, materialeigenschaften) und können später auch mit Biomen, Regionen und Rezepten verknüpft werden.

## Tabellarische Übersicht
```base
filters:
  and:
    - file.folder.startsWith("01_Welt/02_Komponenten")
views:
  - type: table
    name: Table
    filters:
      and:
        - file.name != "02_Komponenten"
    order:
      - kategorie
      - file.name
      - biome
      - merkmale
    sort:
      - property: kategorie
        direction: ASC
      - property: biome
        direction: ASC
    columnSize:
      note.biome: 419
      note.merkmale: 791
    markers: number

```
