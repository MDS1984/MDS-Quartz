---
type: region
biome:
  - "[[Dünen & Sandmeer]]"
  - "[[Ebenen & Steppen]]"
  - "[[Oasen]]"
  - "[[Küste & Brandungszone]]"
  - "[[Karawanenwege & Handelsrouten]]"
  - "[[Hügel]]"
banner_image: https://www.tour-edition.de/media/images/country/75/xl_Oman_Rub%20Al%20Khali_bei%20Salalah_as_tour_332416007_ie.jpeg
---
# Regionsüberblick
## Kurzbeschreibung  
Die Ketzwüste ist eine weite Halb- und Vollwüste aus goldenen Sanden, Oasenstädten, Salzebenen und militärisch gesicherten Handelswegen, in der sich idealisierte Wüstenromantik, elementare Mächte und uralte Bedrohungen überlagern. Sie wirkt vertraut und märchenhaft, ist aber voller fanatischer Schreine, begrabener Tempel und strategischer Festungen.

## Lage & Kontext  
Die Ketzwüste bildet einen großen trockenen Raum Qadiras, der in Teilen aus jener klassischen Wüstenlandschaft besteht, die Außenstehende mit dem Land verbinden: goldene Dünen, Oasen und weiße Kuppelstädte. Nach Osten steigt das Land an, wird erst zur Steppe und geht schließlich in den Tapurwald über. Die Region ist dadurch sowohl Kernland qadirischer Wüstenidentität als auch Übergangszone zwischen Karawanenwelt, Militärmacht und fremdartigen Elementarreichen.

## Impressionen  
**Immer:** Trockene Hitze, goldener Staub, heller Stein, Wind über Sand und Gras, ferne Tierlaute, Salz in der Luft der Ebenen, das Wechselspiel aus Weite und isolierten Lebensinseln.  
**Frühling:** Kurze grüne Schimmer in den Halbtrockenflächen, kühlere Nächte, wandernde Herden, belebte Oasen und sichere Reisezeit.  
**Sommer:** Brennende Sonne, flirrende Horizonte, staubige Winde, überhitzte Routen, schroffe Schatten und gefährlich aktive Wüstenkreaturen.  
**Herbst:** Beste Zeit für Karawanen, klare Sicht, geschäftige Städte, neue Gerüchte aus den Oasen und mehr Bewegung zwischen Steppe und Wüste.  
**Winter:** Kalte Nächte, scharfe Winde, ausgedünnte Reiserouten, ruhige Tage in den Städten und eine fast heilige Stille über den Salzebenen.

## Das prägende Element  
Das prägende Element ist die **Grenze zwischen bewohnbarer Wüste und übernatürlicher Ödnis**. Die Ketz ist nicht einfach leer, sondern voller Oasen, Schreine, Geistermächte und vergessener Tiefen, die nur knapp unter dem vertrauten Bild der Karawanenwüste verborgen liegen.

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

- Warum duldet Qadira Orte wie Hanpa oder Ehur, obwohl dort Mächte verehrt oder beherbergt werden, die anderswo als Gefahr gelten?
    
- Was liegt wirklich unter den Salzebenen verborgen, und warum wurde der Tempel des Ewigen Obelisken dort versiegelt?
    
- Welche Rolle spielen Merev und Yanimer im größeren Netz aus Krieg, Handel und Geheimrouten unter dem Meer?
    

## Fragen an die Figuren

- Wer von euch ist schon einmal mit einer Karawane durch die Ketz gezogen oder in einer Oasenstadt gestrandet?
    
- Wen kennt ihr hier: einen Teppichhändler, einen Offizier, einen Elementardiener, einen Pilger oder einen Söldnerhauptmann?
    
- Was habt ihr in der Ketz zurückgelassen: einen Eid, eine Schuld, ein Relikt, einen Geliebten oder einen toten Kameraden?
    

# Orte & Aufhänger

## Wichtige Orte

- **Ehur** – Stadt der Elementargeister und Zuflucht für Elementargeistartige; ein politisch und metaphysisch heikler Ort.
    
- **Hanpa** – isoliertes Dorf mit Pazuzu-Schrein und schützenden Windstürmen; gefährlich, fanatisch und schwer anzugreifen.
    
- **Khundurai** – berühmtes Zentrum der Teppichkunst, in dem magische Flugteppiche verborgen gefertigt werden können.
    
- **Tempel des Ewigen Obelisken** – unter Salzebenen begrabener Tempel mit Gerüchten um ewiges Leben.
    
- **Merev / Yanimer** – mächtige Festungs- und Marinestadt auf einer Felseninsel, militärischer Schlüsselpunkt Qadiras.
    
- **Hawah, Tekeh, Merischai** – weitere Städte und Dörfer für Handel, Frömmigkeit, Hirtenleben und Durchreise.
    

## Aufhänger

- Eine Karawane verschwindet auf dem Weg zwischen Oasen und Salzebenen, und nur seltsame Spuren im Wind bleiben zurück.
    
- Ein Auftraggeber sucht jemanden, der ein altes Befehlswort für einen fliegenden Teppich in Khundurai beschafft.
    
- Gerüchte über den Tempel des Ewigen Obelisken locken Schatzsucher, Kultisten und Militär zugleich an.
    
- Ein Pazuzu-Sturm aus Hanpa weitet sich aus und bedroht eine Handelsroute oder Pilgerstraße.
    
- In den Tunneln unter Yanimer verschwindet ein wichtiger Offizier, Spion oder Diplomat.
    

# Zufallstabellen

## Terrain  
Goldene Dünen, Halbtrockensteppe, ausgedörrte Grasflächen, Salzebenen, Kakteenfelder, Oasen, weiße Kuppelstädte, Felsinseln, Karawanenpfade, windgegerbte Steilhänge.

## Entdeckungen  
Ein halb vergrabener Obelisk, ein magisch gewebter Teppich, versteinerte Spuren eines Wüstenwurms, ein alter Schrein im Sand, eine verborgene Quelle, elementare Sigillen, versiegelte Höhleneingänge, alte Militärlager.

## Begegnungen  
Karawanenhändler, Pilger, Söldner, Hirten, Elementargeister, Elementargeistartige, Teppichknüpfer, Militärpatrouillen, Maftets, Wüstenuntote, Troglodyten, reisende Gläubige.

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

Die Ketzwüste ist bewohnt von Gläubigen, Händlern, Hirten, Kunsthandwerkern und Soldaten, die zwischen Oasen, Städten und Karawanenwegen leben. Unter den nichtmenschlichen Gefahren und Mächten finden sich Blaue Drachen, Elementargeister, Gargylen, Maftets, Riesentausendfüßler, Riesenwüstenwürmer, Schreckensfledermäuse, Troglodyten und Wüstenuntote; dazu kommen alltäglichere, aber nicht minder gefährliche Tiere wie Vipern, Skorpione und Hyänen.

# Besonderheiten

Die Ketzwüste ist wahrscheinlich die „ikonischste“ qadirische Region, aber gerade deshalb spannend, weil unter dem vertrauten Bild viel Fremdes und Gefährliches liegt. Die Region verbindet Oasenromantik, Militärmacht, verbotene Kulte, elementare Diplomatie und archaische Ruinen auf engem Raum. Als regionale Regel eignet sich hier besonders: **Jeder sichere Ort ist eine Ausnahme; zwischen zwei Zufluchten gehört die Wüste jemand anderem.**