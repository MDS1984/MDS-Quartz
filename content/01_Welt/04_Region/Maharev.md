---
type: region
biome:
  - "[[Dschungel]]"
  - "[[Hügel]]"
  - "[[Ebenen & Steppen]]"
  - "[[Fluss- und Wadi-Täler]]"
  - "[[Mangroven & Brackwassersümpfe]]"
  - "[[Dünen & Sandmeer]]"
banner_image: https://www.naturespots.net/media/k2/items/cache/9eb5fe68e2752a991d20ff91a1cdb543_L.jpg
---
# Regionsüberblick 
## Kurzbeschreibung  
Maharev ist Qadiras fruchtbare Dschungel- und Flussregion, ein geschütztes, reiches Nahrungsland zwischen Bergen, Flüssen und undurchdringlichem Süden. Hinter der scheinbaren Ruhe liegt eine Region voller Expeditionen, Grenzkonflikte, rivalisierender Kulte und gefährlicher Wildnis.

## Lage & Kontext  
Maharev liegt zwischen den Zhobergen und dem Maharev-Fluss im Westen und dem Merazstrom im Osten; im Süden schützt eine kaum passierbare Wüste die Region zusätzlich. Sie ist das landwirtschaftliche Rückgrat Qadiras und zugleich kulturell enger mit Kelesch verbunden als viele andere qadirische Gebiete. Außenstehenden erscheint die Region oft wie ein abgelegener, fast übersehener Randraum — in Wahrheit ist sie ein zentraler Versorger und ein politisch interessanter Puffer.

## Impressionen  
**Immer:** Feuchte Luft, dichter Grünwuchs, Flussgeräusche, Tierstimmen, süßer Pflanzen- und Gewürzgeruch, schweres Blätterdach, langsame Bewegung des Wassers, eine friedliche Oberfläche mit unterschwelliger Wildnis.  
**Frühling:** Überschwemmte Ufer, wuchernde Saaten, summende Insekten, frische Blätter, Arbeitsfieber auf den Feldern.  
**Sommer:** Schwüle Hitze, reife Früchte, Gewitter am Horizont, schattenreiche Pfade, voller Erntebetrieb und gefährlich aktiver Dschungel.  
**Herbst:** Erntedank, Handelskarawanen, getrocknete Gewürze, goldene Felder, ruhigerer, aber angespannter Rhythmus.  
**Winter:** Mild im Vergleich zum Rest Qadiras, feuchte Kühle, Nebel über den Flüssen, weniger Verkehr, aber mehr Gerüchte und stille Bedrohungen.

## Das prägende Element  
Das prägende Element ist der **lebensspendende, aber unerforschte Dschungel**: Maharev nährt ganz Qadira, doch seine Wildnis ist voller alter Gefahren, Geheimnisse und rivalisierender Mächte. Die Region ist also zugleich Kornkammer und Grenzraum.

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

- Warum lässt Qadira Maharev so ungestört wachsen, obwohl die Region so reich ist?
    
- Was verschweigt die Region über den Ursprung der Grünen Mutter und der fleischfressenden Pflanzen?
    
- Wer kontrolliert wirklich die Wege zwischen den Ernten, den Städten und den verborgenen Dschungelzonen?
    

## Fragen an die Figuren

- Wer von euch hat schon einmal eine Ernte, Expedition oder Karawane in Maharev begleitet?
    
- Wen kennt ihr hier: einen Händler, einen Forscher, einen Priester oder einen Grenzoffizier?
    
- Was habt ihr in Maharev verloren: eine Karte, ein Relikt, einen Verwandten, einen Auftrag?
    

# Orte & Aufhänger

## Wichtige Orte
- **Qaharid** – Türkisstadt, Handels- und Handwerkszentrum, kultureller Knotenpunkt.
- **Rikhist** – raues Grenzdorf, Zentrum der Rovagugverehrung, sozial und militärisch brandgefährlich.
- **Sanmeschul** – große Stadt der Bildung, Verwaltung oder wohlhabenden Gesellschaft.
- **Al-Hiraf / Isa / Nirfan / Raschiz** – als weitere Ortschaften für Höfe, Lager, Schulen, Plantagen oder Außenposten.

## Aufhänger
- Eine neue Expedition in den Dschungel verschwindet, bevor sie die erste Karte zurückschicken kann.
- Zwischen Qaharid und Rikhist eskaliert ein Konflikt um Religion, Grenzsicherung oder geheime Pilgerströme.
- Eine Ernte, eine Handelsroute oder ein wichtiger Kupfer-/Türkisfund wird von Monstern, Kultisten oder rivalisierenden Mächten bedroht.

# Zufallstabellen

## Terrain  
Flussufer, Dschungelpfade, Terrassenfelder, Kupferminen, bewaldete Hügel, Sümpfe, Regenwald, Grenzsteine, schmale Hänge, verlassene Ruinen.

## Entdeckungen  
Seltene Gewürzpflanzen, alte Tempelreste, versteckte Tierpfade, zerbrochene Dschinn-Siegel, türkisblaue Adern im Fels, verlassene Feldstationen, verschüttete Opferplätze.

## Begegnungen  
Bauern mit Erntewagen, Forscher mit Trägern, Dschungelriesen auf Wanderung, Dschungeldrakas, Pilger der Weißen Feder, Roidira-Anhänger, Grenzsoldaten, Orkstämme aus den Bergen.

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

Maharev ist geprägt von einer ungewöhnlich breiten Mischung aus **Bauern, Forschern, Künstlern, Studenten, Händlern und Militärs**. Dazu kommen die gefährlichen, aber ikonischen Bewohner des Dschungels: Dschungeldrakas, Dschungelriesen, Qlippoth, giftige Frösche, Mantikore, Wyverns, Schreckenskrokodile und riesige Wüstenwürmer.

# Besonderheiten

Maharev wirkt nach außen friedlich und fruchtbar, ist aber in Wahrheit ein **Dreiklang aus Nahrung, Wissen und Wildnis**. Qaharid kann als kulturelles Zentrum und Qlippoth für gefährliche Mystik stehen, während Rikhist die Region mit fanatischer Gegenreligion und Grenzverfall auflädt. Als regionale Regel könnte gelten: **Je tiefer man in den Dschungel geht, desto stärker verschiebt sich die Region von Ackerland zu Urwildnis und von Handel zu Mythos.**