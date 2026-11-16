---
type: region
biome:
  - "[[Gebirge]]"
  - "[[Hügel]]"
  - "[[Fluss- und Wadi-Täler]]"
  - "[[Canyons & Schluchten]]"
  - "[[Karawanenwege & Handelsrouten]]"
  - "[[Verlassene Ruinen & Steinwüsten]]"
banner_image: https://peakvisor.com/photo/SD/Saudi-Arabia-forest-mountains.jpg
---
# Regionsbeschreibung
## Kurzbeschreibung  
Paschman ist eine gebirgige, überraschend fruchtbare Region aus Schnee, Flüssen, Karawanenstädten und alten Ruinen, in der Handel, Kunst, Militär und uralte Gefahren dicht beieinanderliegen. Die spektakulären Landschaften nähren Kreativität, aber auch Rivalität, Geheimnisse und sehr harte Grenzen.
## Lage & Kontext  
Die Region wird im Norden vom Ladanfluss und im Süden vom Paschman begrenzt. Sie bildet einen wichtigen Übergang nach Kelesch und ist für Reisende oft der letzte sichere Abschnitt vor dem großen Osten. Trotz ihrer Schönheit ist sie nicht friedlich: verlassene Städte, finstere Unterwelten und politische Spannungen machen sie zu einem Raum, in dem Wege, Grenzen und alte Mächte ständig miteinander konkurrieren.
## Impressionen  
**Immer:** Kühle Bergluft, schneebedeckte Gipfel, klare Flüsse, der Duft von Holz und Kräutern, Glocken und Karawanengeräusche, weite Ausblicke, stille Gefahr unter schöner Oberfläche.  
**Frühling:** Schmelzwasser, üppige Vegetation, Erdrutsche an Hängen, lebhafte Städte, Karawanen in Bewegung, mehr Jagd und Sammeln.  
**Sommer:** Klare Sicht, volle Handelswege, blühende Bergflanken, intensive Handwerksarbeit, Feste und kunstvolle Aufführungen.  
**Herbst:** Kühler werdende Nächte, reifende Vorräte, dichter Handel, Nebel in den Tälern, erste Schneefälle in den Höhen.  
**Winter:** Schnee, harte Pässe, eingeschränkte Wege, Lagerfeuer, isolierte Städte und ein stärkeres Gefühl von Abgeschiedenheit.
## Das prägende Element  
Das prägende Element ist die **schöne, gefährliche Hochlandgrenze**: Paschman ist ein Ort, an dem Aussicht und Absturz, Kultur und Verfall, Handel und Ruine direkt nebeneinanderliegen. Die Region inspiriert, aber sie vergisst auch nichts.
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
- Warum ist eine so schöne Region politisch und mythologisch so anfällig für Ruinen, Monster und verborgene Schrecken?
- Was bewahren die alten Städte, Schreinruinen und Unterwelten unter Khoka wirklich?
- Wer kontrolliert die Karawanenwege zwischen den sicheren Städten und den gefährlichen Bergzonen?
## Fragen an die Figuren
- Wer von euch hat schon einmal eine Karawane durch Paschman begleitet oder hier einen Winter verbracht?
- Wen kennt ihr hier: einen Architekten, eine Musikerin, einen Rüstungsschmied, einen Wahrsager oder eine Händlerfamilie?
- Was habt ihr in Paschman verloren: einen Auftrag, ein Lied, einen Rivalen, ein Relikt oder einen Namen?
# Orte & Aufhänger
## Wichtige Orte
- **Lopul** – große Karawanenstadt an der Oase Sihbons Teich, im heißesten Teil der Region.
- **Khoka** – letzter Halt für Reisende Richtung Kelesch, geographischer und politischer Randpunkt.
- **Al-Baschir** – verlassene Ruinenstadt voller Gerüchte über Schätze und verzauberte Harpyien.
- **Koor** – alte Schmiedestadt mit Ruinen, zerbrochenem Metall und einer rätselhaften Wächternaga.
- **Kamawgyar-Schrein** – verlassener Irori-Schrein mit verborgener Harpyienpräsenz.
- **Magrevor** – Unterweltbereich mit Magmagrube, Höllenportal und duergarischem Sklavennetzwerk.
## Aufhänger
- Eine Karawane muss durch die trockenste und heißeste Zone begleitet werden, bevor Vorräte oder Wasser ausgehen.
- In Al-Baschir werden Schätze, Flüche oder harpyische Intrigen gesucht.
- Der Satrap will wissen, ob Samraf al-Hadari in Lopul loyal bleibt oder zu mächtig wird.
- Unter Khoka führt eine Spur in die Finsterlande und zu einem Portal nach Malebolge.
- Ein alter Schrein, eine Ruinenstadt oder eine Schmiedestätte droht, neue Gefahren freizusetzen.
# Zufallstabellen
## Terrain  
Schneegipfel, Bergwiesen, steile Hänge, Passstraßen, Oasen, trockene Hochflächen, Flusstäler, Ruinenhügel, Schmiedeviertel, Felsplateaus.
## Entdeckungen  
Zerbrochene Bronzeobjekte, alte Schmiedegeheimnisse, vergessene Karten, versteckte Pfade, Harpyiennester, verborgene Schreine, Oasenquellen, Naga-Spuren, Ruinenlager, alte Karawanenmarkierungen.
## Begegnungen  
Architekten, Astrologen, Bauern, Baumeister, Handwerker, Ingenieure, Jäger, Künstler, Musiker, Rüstungsschmiede, Schriftsteller, Wahrsager, Karawanenführer, Harpyien, Duergar, Wölfe, Ogerspuren, Bergwächter.
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
Die Region wird von Bauern, Architekten, Astrologen, Baumeistern, Handwerkern, Ingenieuren, Jägern, Künstlern, Musikern, Rüstungsschmieden, Schriftstellern und Wahrsagern bewohnt. Dazu kommen Duergar, Harpyien, Lamien, Luchse, Nagas, Pferde, Pferdegreifen, Riesenaffen, Rieseneidechsen, Schreckenskrähen, Wölfe und Ziegen.
# Besonderheiten
Paschman ist eine Region der **sichtbaren Schönheit mit verborgener Verderbnis**. Sie lebt von Karawanen, Talenten, Bergbau und Kunst, aber auch von Ruinen, Unterwelten und gefährlichen Grenzen; gerade deshalb eignet sie sich hervorragend für Kampagnen über Reise, Rivalität und alte Geheimnisse. Als regionale Regel passt hier besonders: **Wer in Paschman einen sicheren Weg kennt, besitzt Macht.**

