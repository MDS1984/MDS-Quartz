---
type: region
biome:
  - "[[Dünen & Sandmeer]]"
  - "[[Salzwüste]]"
  - "[[Oasen]]"
  - "[[Salzhügel & Salzberge]]"
  - "[[Karawanenwege & Handelsrouten]]"
  - "[[Verlassene Ruinen & Steinwüsten]]"
  - "[[Heilige Orte]]"
banner_image: https://images.takeshape.io/86ce9525-f5f2-4e97-81ba-54e8ce933da7/dev/edbabbc5-b342-4169-a0e7-ca56b6675590/Sandstone%20plateau%2C%20Hisma%20Desert%20%E2%80%93%20NEOM%2C%20Saudi%20Arabia%20%7C%20The%20NEOM%20Nature%20Reserve%20region%202%20neom-39n8YVSn0d4-unsplash.jpg?auto=compress%2Cformat&w=1600
---
# Regionsbeschreibung

## Kurzbeschreibung  
Die Merazwüste ist Qadiras endlose Südwüste aus goldenen Sanddünen, verlorener Geschichte und uraltem Verderben. Sie trennt das Reich von Kelesch, bewahrt Ruinen unter tödlicher Hitze und wird von Oasen, Reiterstämmen und unheimlichen Mächten durchzogen.

## Lage & Kontext  
Die Merazwüste liegt im südlichen Qadira und markiert die große Trennlinie zum übrigen Kelesch. Einst war sie eine fruchtbare Savanne, bis die vier Herolde des Staubes sie in eine Sandwüste verwandelten; seitdem trägt sie die Last zerstörter Zivilisationen und vergessenen Bösen. Trotz ihrer Leere ist sie nicht leer: Oasen, Untergrundstädte, Ruinen und Reiterwege machen sie zu einem Raum aus Überleben, Handel und Geheimnis.

## Impressionen  
**Immer:** Trockene Gluthitze, goldener und weißer Sand, knöcherne Baumgerippe, flirrendes Licht, Windstöße, knirschende Stille, Einsamkeit mit dem Gefühl alter Schuld.  
**Frühling:** Kürzere, mildere Hitzephasen, Karawanenverkehr, Blüte in geschützten Oasen, Herden an Wasserstellen, mehr Bewegung zwischen den Siedlungen.  
**Sommer:** Tödliche Mittagshitze, flimmernde Horizonte, Staubstürme, erschöpfte Tiere, harte Reisebedingungen, besonders aktive Wüstengefahren.  
**Herbst:** Beste Reisezeit, mehr Händler und Söldner unterwegs, klare Nächte, gespannte Ruhe vor dem Winter, gute Saison für Expeditionen.  
**Winter:** Kühler, aber immer noch trocken, lange Nächte, starke Winde, mehr Lagerleben als Reisen, Gerüchte über Ruinen und Geister werden lauter.

## Das prägende Element  
Das prägende Element ist die **verwandelte Landschaft der Erinnerung**: eine Wüste, die einst Leben trug und nun nur noch als Grab der Vergangenheit existiert. Jede Oase, jedes Bauwerk und jede Karawanenroute steht im Schatten dieser verlorenen Fruchtbarkeit.

# Komponenten
~~~notetabs

---begintab
header: Jagen

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
---closetab

---begintab
header: Fischen

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
---closetab


---begintab
header: Materialien

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
---closetab

---begintab
header: Kräuter

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
---closetab

~~~
# Fragen

## Fragen an die Welt

- Was war die Merazwüste vor den Herolden des Staubes, und warum wurde sie so vollständig verdammt?
    
- Welche Geheimnisse schützen die Schedus um die alten Bauwerke und Ruinen?
    
- Was liegt wirklich hinter den unterirdischen Städten, Oasen und den Wegen der Reiterstämme?
    

## Fragen an die Figuren

- Wer von euch kennt die Wüste aus einer Karawane, einem Feldzug oder einer verlorenen Expedition?
    
- Wen kennt ihr hier: einen Pferdezüchter, einen Wüstenkrieger, eine Kirchenverwalterin, einen Archäologen oder einen Oasenältesten?
    
- Was habt ihr in der Meraz zurückgelassen: eine Karte, ein Grab, ein Pferd, einen Eid oder einen Toten?
    

# Orte & Aufhänger

## Wichtige Orte

- **Dimayen** – Oasenstadt mit eingestürzten Bewässerungstunneln, ankhegs und intelligenten Schakalen.
    
- **Ihalar** – große unterirdische Stadt im Stil der Khattibi, mit Gärten, Lichtschächten und lebendiger Handelskultur.
    
- **Jezonna-Oase** – Heimat eines Wüstenriesenstammes, wichtig für Karawanenschutz und lokale Macht.
    
- **Qumarin** – geheime Ruinenlage, nur wenigen Girtablilus bekannt.
    
- **Sonnengebleichter Turm** – unheimlicher Knochenbau nördlich von Dimayen, Anziehungspunkt für Daimonen.
    
- **Heger, Husanah, Izzet** – weitere Städte als Ankerpunkte für Handel, Verwaltung, Reiterei und Grenzleben.
    

## Aufhänger

- Eine Karawane verschwindet auf der Route zwischen Ihalar und Dimayen, und nur Ruinenmarkierungen bleiben zurück.
    
- Archäologen suchen Schutz oder Führer für eine Expedition zu Qumarin oder dem Sonnengebleichten Turm.
    
- Ein Wüstenriesenstamm bittet um Hilfe gegen eine übernatürliche Bedrohung oder um politische Anerkennung.
    
- Ein altes Relikt aus der Merazwüste scheint mit den Herolden des Staubes verbunden zu sein.
    
- In einer Oase eskaliert ein Konflikt zwischen lokalen Hirten, Kirchenbeamten und Räuberbanden.
    

# Zufallstabellen

## Terrain  
Goldene Dünen, weiße Sandfelder, Oasenbecken, trockene Savannenreste, Knochenwälder, Ruinenhügel, unterirdische Gärten, steile Dünenkämme, Karawanenpfade, Felsinseln im Sandmeer.

## Entdeckungen  
Vergrabene Ruinen, alte Wasserkanäle, Knochenstatuen, Pferdespuren, versiegelte Grabstätten, Ruinenkarten, fremde Handelszeichen, Schlangensymbole, halb verschüttete Tempel, Oasen mit versteckten Zugängen.

## Begegnungen  
Archäologen, Eremiten, Hirten, Kirchenbeamte, Krieger, Pferdezüchter, Räuber, Wüstendruiden, Elementargeistartige, Wüstenriesen, Schedus, Girtablilus, Schakale, Sphingen.

## Gefahren  
```base
filters:
  and:
    - file.inFolder("01_Welt/05_Gefahren")
    - type == "Herausforderung"
    - "list(biome).filter(list(this.biome).contains(value)).length > 0 "
views:
  - type: list
    name: Gefahren – alle Biome dieser Region
    order:
      - file.name
    columns:
      - name as Komponente
      - biome as Biome
    markers: number
```

# Bewohner & Monster

Die Merazwüste ist geprägt von Archäologen, Elementargeistartigen, Eremiten, Hirten, Kirchenverwaltungsbeamten, Kriegern, Pferdezüchtern, Räubern und Wüstendruiden. Dazu kommen Basilisken, Behire, Dämonen, Daimonen, Dschanni, Dschinni, Elementarrösser, Girtablilus, Ifriti, Kamele, Lamien, Medusen, Phönixe, riesige Wüstenwürmer, Schedus, Sphingen, Wüstenriesen, Skorpione, Wespen und Wüstenuntote.

[[Edimmu]]

# Besonderheiten

Die Merazwüste ist eine Region des **Verlusts, der Wege und der verborgenen Gegenwarten**. Ihre Stärke liegt nicht in städtischer Dichte, sondern in Karawanen, Pferdekulturen, Oasen, unterirdischen Zufluchten und gefährlichen Ruinen; zugleich macht sie die Nähe zu Daimonen, Relikten und den Schatten der Vergangenheit zu einem idealen Raum für Expeditionen und Omen. Als regionale Regel passt hier besonders: **Alles, was in der Meraz lange genug verborgen bleibt, wird entweder heilig, gefährlich oder beides.**