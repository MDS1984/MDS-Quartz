---
type: region
biome:
  - "[[Dünen & Sandmeer]]"
  - "[[Sandige Halbinseln]]"
  - "[[Ebenen & Steppen]]"
  - "[[Oasen]]"
  - "[[Küste & Brandungszone]]"
  - "[[Karawanenwege & Handelsrouten]]"
  - "[[Salzwüste]]"
cssclasses:
  - base no header
banner_image: https://www.domina.it/wp-content/uploads/sites/360/2026/04/Sinai-peninsula-1366x768.jpg
---




# Regionsüberblick 
## Kurzbeschreibung  
Die Alavah-Halbinsel ist eine salzdurchzogene Wüstenküste aus Handelsstädten, Sklavenmärkten, gefährlichen Inseln und machtvollen, oft fremdartigen Kräften. Sie ist reich, heiß, politisch verworren und voller Gegensätze zwischen Luxus und Verfall.

## Lage & Kontext  
Südlich der Zhoberge zieht sich die Alavah-Halbinsel als große Küstenlandmasse entlang einer schmalen Wasserstraße. Im Süden liegt die fruchtbarere Smaragdküste mit ihren Städten und Feldern; der zentrale Teil ist eine glitzernde, unbewohnbare Kristall- und Salzwüste. Die Halbinsel ist eng mit Seefahrt, Sklavenhandel, Inselbedrohungen und den Machtspielen Qadiras verknüpft.

## Impressionen  
**Immer:** Heiße Luft, Salzgeruch, blendendes Licht, glitzernder Sand, ferne Möwen oder Wind, das Knirschen von Schuhen auf hartem Boden, das Gefühl von Reichtum und Gefahr zugleich.  
**Frühling:** Kühlere Morgen, frische Brisen vom Meer, geschäftige Häfen, beginnende Karawanen, erste Gartenblüten in den geschützten Zonen.  
**Sommer:** Unerträgliche Hitze, flirrende Luft, gleißender Sand, überfüllte Märkte, schweißnasse Kleidung, Schatten als kostbarste Ware.  
**Herbst:** Ruhigere See, dichter Handel, Ernte in den südlichen Feldern, politische Spannungen in den Städten, mehr Gerüchte über die Inseln.  
**Winter:** Mild an der Küste, aber rau und trocken im Inneren; klare Sicht, scharfer Wind, intensiver Schiffsbetrieb, weniger Reisende, mehr Intrigen.

## Das prägende Element  
Das prägende Element ist die **Küste der Gegensätze**: Reichtum und Sklaverei, Garteninseln und Todeswüste, offene Handelsstädte und verborgene Machtzentren. Die Halbinsel wirkt wie ein Ort, an dem jede Ware, jede Person und jede Loyalität einen Preis hat.

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

- Warum toleriert Qadira die Machtstrukturen und Grausamkeiten dieser Halbinsel trotz ihres enormen Werts?
    
- Was verbinden die Inseln der Gefahren, die Bronzeschwestern und die finsteren Handelswege wirklich miteinander?
    
- Welche alten Mächte liegen unter der scheinbar glanzvollen Oberfläche der Küstenstädte?
    

## Fragen an die Figuren

- Wer von euch hat schon einmal auf einer der Inseln der Gefahren, in Sedeq oder bei Wyos Rast gearbeitet oder gekämpft?
    
- Wen kennt ihr hier: eine Händlerfamilie, eine Matriarchin, einen Sklavenhändler, einen Schmuggler oder einen Schiffsbauer?
    
- Was habt ihr in Alavah verloren: einen Namen, eine Schuld, ein Schiff, einen Gefangenen oder einen Handel?
    

# Orte & Aufhänger

## Wichtige Orte

- **Sedeq** – Sklavenmarkt, Handelszentrum und moralisch verrotteter Luxusort.
    
- **Uschumgal** – reiche, geheimnisvolle Stadt unter dem Einfluss mächtiger Frauen oder Bronzedrachen.
    
- **Wyos Rast** – Garteninsel und Harem, Ort von Tribut, Schutz und höfischem Luxus.
    
- **Yalakhin** – die Klagende Stadt, Zentrum des Yahaiya-Kultes.
    
- **Erukhs Zelte** – Zeltstadt um einen verbannten Elementargeist mit Aufgaben statt Geschenken.
    
- **Flammenzitadelle** – ruinöses oder verborgenes Molochzentrum mit düsterem Rekrutierungsnetz.
    
- **Neue Brandlande** – von Divs heimgesuchte Küstenzone im Süden.
    
- **Ayesch, Jawafiq, Sadiyeh, Sukri, Uschumgal** – weitere wichtige Städte für Handel, Söldner, Schiffbau und Machtpolitik.
    

## Aufhänger

- Ein Schiff verschwindet zwischen Halbinsel und Inseln der Gefahren, und nur wenige wollen offen darüber reden.
    
- Ein Patron oder Handelshaus sucht Leute, die Zugang zu Sedeq, Uschumgal oder Erukhs Zelte bekommen.
    
- Die SC werden in Konflikte zwischen Sklavenhandel, Reliktjagd, Drachenmacht und Kultintrigen hineingezogen.
    

# Zufallstabellen

## Terrain  
Salzwüste, Kristallfelder, Küstenklippen, Hafenmauern, Gartenanlagen, Dünen, Flachküste, Inselstrände, Felsrücken, Karawanenwege.

## Entdeckungen  
Verlassene Karawanenlager, verborgene Gartenhöfe, versunkene Kaianlagen, Drachenzeichen, verfluchte Marktstände, alte Tributlisten, Kristalladern, geheime Schifffahrtsrouten.

## Begegnungen  
Sklavenhändler, Schmuggler, Schiffsbauer, Wüstenfeen, Divs, Sphingen, Seefahrer, Soldaten, Bronzeschwestern, Kultanhänger, Karawanenführer.

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

Die Halbinsel ist bevölkert von Bergarbeitern, nomadischen Viehtreibern, Schiffsbauern, Sklavenhändlern und Soldaten. Dazu kommen Bronze- und Messingdrachen, Divs, Halb-Ork-Räuber, Schaitane, Sphingen, Wüstenfeenwesen, Wüstenuntote sowie Ungeziefer wie Wespenschwärme und Wüstenspinnen.

# Besonderheiten

Die Alavah-Halbinsel ist ein Ort, an dem Reichtum und Verderben nebeneinander existieren. Die Smaragdküste bietet fruchtbare Städte und Handel, während das Zentrum durch Hitze und Kristallsand fast unbewohnbar wird; zugleich machen die Inseln der Gefahren, die Bronzeschwestern von Uschumgal und die dunklen Mächte um Sedeq die Region zu einem politischen und übernatürlichen Brennpunkt. Als regionale Regel passt hier besonders gut: **Jeder Zugang ist kontrolliert, jeder Schutz kostet etwas, und fast jeder sichere Ort ist mit einem Preis oder einer Loyalität verbunden.**
