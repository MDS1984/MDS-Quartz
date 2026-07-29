---
type: region
biome:
  - "[[Hügel]]"
  - "[[Ebenen & Steppen]]"
---

# [Regionsname]

## Kurzbeschreibung
[Ein Satz, der Ort, Stimmung und Besonderheit beschreibt.]

## Lage & Kontext
[Wo liegt die Region, woran grenzt sie, welche Rolle spielt sie in der Welt?]

## Impressionen
### Immer
- [Geräusch, Licht, Geruch, Bewegung, Grundstimmung]

### Frühling
- [...]

### Sommer
- [...]

### Herbst
- [...]

### Winter
- [...]

## Das prägende Element
[Das zentrale Phänomen, das die Region besonders macht. Z. B. ein verfluchter Brunnen, ein ewiger Wind, eine heilige Salzebene.]

## Komponenten
### Jagen
```base
filters:
  and:
    - file.inFolder("01_Welt/02_Komponenten")
    - type == "komponente"
    - kategorie == "jagd"
    - "list(biome).filter(list(this.biome).contains(value)).length > 0 "
views:
  - type: list
    name: Jagen – alle Biome dieser Region
    order:
      - file.name
    columns:
      - name as Komponente
      - biome as Biome
    markers: number
```

### Fischen
```base
filters:
  and:
    - file.inFolder("01_Welt/02_Komponenten")
    - type == "komponente"
    - kategorie == ["fischen"]
    - "list(biome).filter(list(this.biome).contains(value)).length > 0 "
views:
  - type: list
    name: Jagen – alle Biome dieser Region
    order:
      - file.name
    columns:
      - name as Komponente
      - biome as Biome
    markers: number
```

### Materialien
```base
filters:
  and:
    - file.inFolder("01_Welt/02_Komponenten")
    - type == "komponente"
    - kategorie == ["materialkunde"]
    - "list(biome).filter(list(this.biome).contains(value)).length > 0 "
views:
  - type: list
    name: Jagen – alle Biome dieser Region
    order:
      - file.name
    columns:
      - name as Komponente
      - biome as Biome
    markers: number

```

### Kräuter
```base
filters:
  and:
    - file.inFolder("01_Welt/02_Komponenten")
    - type == "komponente"
    - kategorie == ["kraeuterkunde"]
    - "list(biome).filter(list(this.biome).contains(value)).length > 0 "
views:
  - type: list
    name: Jagen – alle Biome dieser Region
    order:
      - file.name
    columns:
      - name as Komponente
      - biome as Biome
    markers: number
```

## Fragen
### Fragen an die Welt
- [Warum ...?]
- [Was geschah ...?]
- [Wer kontrolliert ...?]

### Fragen an die Figuren
- [Wer von euch ...?]
- [Wen kennt ihr hier ...?]
- [Was habt ihr hier verloren ...?]

## Orte & Aufhänger
### Wichtige Orte
- [Ort 1]
- [Ort 2]

### Aufhänger
- [Problem oder Gerücht]
- [Bedrohung oder Auftrag]
- [Geheimnis oder Fund]

## Zufallstabellen
### Terrain
- [...]
### Entdeckungen
- [...]
### Begegnungen
- [...]

## Gefahren
[Umweltgefahren, Reisegefahren, soziale Gefahren.]

## Bewohner & Monster
[Kurze Übersicht oder einzelne Einträge.]

## Besonderheiten
[Optionaler Abschnitt für Rituale, Handel, Legenden oder regionale Regeln.]