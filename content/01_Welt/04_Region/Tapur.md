---
type: region
biome:
  - "[[Dschungel]]"
  - "[[Quellen]]"
  - "[[Ebenen & Steppen]]"
banner_image: https://media.hamshahrionline.ir/d/2023/07/18/4/4864242.jpg?ts=1689660186000
---
# Regionsbeschreibung
## Kurzbeschreibung  
Tapur ist Qadiras Wald- und Savannenregion, ein Übergangsraum zwischen Wüste und Gebirge, in dem Nutzholz, Kräuter, Gewürze und stiller Informationshandel wichtiger sind als höfische Politik. Die Region wirkt abgeschieden und eher provinziell, verbirgt aber in ihren Wäldern gefährliche Wildnis, Spione und eine langsam vorrückende Wüste.
## Lage & Kontext  
Tapur trennt die Ketzwüste von den Ebenen westlich der Zhoberge. Im Osten liegt eine noch recht offene Savanne, während der eigentliche Tapurwald sich in einen trockeneren Norden und einen dichten, wilderen Süden teilt. Die Region ist nur leicht besiedelt, politisch eher zurückhaltend und für viele Qadirii eine Randzone, obwohl sie als Holz-, Kräuter- und Geheimnisland durchaus wichtig ist.
## Impressionen  
**Immer:** Harzgeruch, Schatten unter dichtem Blätterdach, Vogelrufe, feuchte Erde, Holzknacken, helle Lichtflecken im Laub, ein Wechsel aus kultivierten Randzonen und wilder Tiefe.  
**Frühling:** Starkes Pflanzenwachstum, reger Holzeinschlag, frische Kräuter, Tierbewegung, mehr Fluss- und Sumpfgeräusche.  
**Sommer:** Schwüle Hitze, dichte Vegetation, Insekten, reiche Gerüche, viel Leben und zugleich hohe Gefahr durch Tiere und Pflanzen.  
**Herbst:** Ernte von Kräutern und Früchten, ruhigeres Tempo, Holztransporte, Nebel in den tieferen Bereichen, mehr Spuren von Wild und Räubern.  
**Winter:** Trockenere Luft im Norden, feuchtere Kühle im Süden, weniger Reiseverkehr, bessere Sicht auf Pfade und Grenzspuren.
## Das prägende Element  
Das prägende Element ist die **langsame Verschiebung von Wald zu Wüste**. Tapur ist ein Gebiet, das nicht nur zwischen Landschaftstypen liegt, sondern auch zwischen Kultur, Politik und dem Einfluss der vorrückenden Ketzwüste.
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
- Warum breitet sich die Ketzwüste aus, und wer profitiert davon oder leidet darunter?
- Was steckt hinter dem Sandsturm von Hatavit, und wer oder was hat ihn ausgelöst?
- Welche Rolle spielt Tapur als stiller Grenzraum zwischen Wüste, Wald und den Machtzentren Qadiras?
## Fragen an die Figuren
- Wer von euch kennt den Wald von Holzarbeit, Jagd, Schmuggel oder einem verdeckten Auftrag?
- Wen kennt ihr hier: einen Färber, Holzfäller, Kräuterkundler, Kürschner, Späher oder Spion?
- Was habt ihr in Tapur verloren: ein Lager, einen Kontakt, ein Geheimnis, eine Karte oder eine Spur?
# Orte & Aufhänger
## Wichtige Orte
- **Hatavit** – Holzfällerlager, nach einem rätselhaften Sandsturm abgeschnitten.
- **Tafinyah** – geheimer Außenposten des Geheimdienstes von Kelesch.
- **Weitere kleine Städte und Dörfer** in Nord- und Süd-Tapur als Randorte, Sammelplätze und Verstecke.
## Aufhänger
- Das Lager Hatavit hat den Kontakt verloren; die SC sollen herausfinden, ob es Naturkatastrophe, Sabotage oder Befreiung war.
- Ein Geheimdienstaußenposten braucht diskrete Hilfe, um in Tapur ein Netzwerk oder eine Bedrohung zu verfolgen.
- Die langsame Ausbreitung der Ketzwüste bedroht Holzgewinnung, Dörfer oder einen wichtigen Pfad.
- Im Südwald verschwinden Jäger, Kräutersammler oder Späher, und die Spur führt zu Feenwesen oder Pflanzengefahren.
# Zufallstabellen
## Terrain  
Dichter Wald, trockener Nordwald, Savannenrand, Sümpfe, Lichtungen, Holzfällerlager, Wurzelwerk, Flussläufe, Randdünen, feuchte Senken.
## Entdeckungen  
Verlassene Lager, befreite Sklaven, alte Holzmarken, geheime Pfade, giftige Pflanzen, Färberpflanzen, Tierfährten, Spuren von Sandstürmen, verdeckte Beobachtungsposten.
## Begegnungen  
Färber, Holzfäller, Kräuterkundler, Kürschner, Möbelschreiner, Späher, Spione, Drakas, Feenwesen, Grüne Drachen, Leoparden, Parde, Spriggane.
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
Die Region ist nur leicht besiedelt und wird von Färbern, Holzfällern, Kräuterkundlern, Kürschnern, Möbelschreinern, Spähern und Spionen geprägt. Dazu kommen Drakas, Feenwesen, Grüne Drachen, Leoparden, Parde, Schreckenswildschweine, Spriggane und Vipernranken.
# Besonderheiten
Tapur ist weniger eine laute Grenzregion als ein **langsamer Konfliktraum**: Holz gegen Wüste, Provinzialität gegen Geheimdienst, Nutzwert gegen Wildnis. Der nördliche Teil ist kultivierbarer und stärker besiedelt, der südliche wilder und gefährlicher; Hatavit und Tafinyah geben der Region zusätzlich einen Hauch von Verlust und verdeckter Macht. Als regionale Regel passt hier besonders: **Was in Tapur verschwindet, kann Holz, Wissen oder Menschen sein.**

