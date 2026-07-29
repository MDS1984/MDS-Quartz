---
type: region
biome:
  - "[[Gebirge]]"
  - "[[Hügel]]"
  - "[[Quellen]]"
  - "[[Canyons & Schluchten]]"
  - "[[Oasen]]"
banner_image: https://peakvisor.com/photo/SD/Saudi-Arabia-Al-Souda-mountains.jpg
---
# Regionsbeschreibung
## Kurzbeschreibung  
Die Nördlichen Zhoberge sind Qadiras ärmster, aber militärisch und strategisch wichtiger Gebirgsrand. Zwischen Passstraßen, Bergwerken, Klöstern und Grenzblicken auf Taldor lebt hier eine Bevölkerung, die mit wenig Komfort, aber viel Spannung im Alltag auskommt.
## Lage & Kontext  
Die Region umfasst das nördliche Ende der Zhoberge samt umliegender Hügel und Ebenen. Sie blickt über die taldanische Grenze hinweg und ist damit nicht nur eine Bergregion, sondern auch eine ständige politische Vorfeldzone. Trotz ihrer relativen Armut ist sie wegen Passstraßen, Ausbildungseinrichtungen und Rohstoffen ein wichtiger Teil Qadiras.
## Impressionen  
**Immer:** Dünne Bergluft, kalter Wind, Glockenklang, Steinpfade, Ausblicke in die Ferne, harte Arbeit, Patrouillen und das Gefühl, am Rand eines größeren Krieges zu stehen.  
**Frühling:** Schneeschmelze, schlammige Wege, sprießende Bergwiesen, reger Handel über die Pässe, mehr Bewegung in Dörfern und Klöstern.  
**Sommer:** Klarer Himmel, schroffe Hitze an den Hängen, helle Tage, Bergarbeit und militärische Übungen, mehr Sicht auf die Grenze.  
**Herbst:** Windig, kühler, Nebel in den Tälern, intensiver Blick über die Grenze, Vorbereitung auf harte Monate.  
**Winter:** Schnee, Eis, gesperrte Pässe, isolierte Siedlungen, konzentrierte Vorräte und ein besonders wachsamer Grenzalltag.
## Das prägende Element  
Das prägende Element ist die **Grenzspannung in der Höhe**: eine Region, die weniger von Reichtum als von Wachsamkeit, Passkontrolle und Kriegsahnung geprägt ist. Der Blick ins Tal und über die Grenze macht die Zhoberge zu einem Ort permanenter Erwartung.
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
- Wann und warum wird aus der stillen Grenzangst tatsächlich Krieg?
- Was schützen die Klöster, Pässe und Satrapiegarnisonen wirklich: die Grenze, ein Geheimnis oder beides?
- Warum ist diese arme Region zugleich so wichtig für Qadiras Sicherheit?
## Fragen an die Figuren
- Wer von euch hat hier Dienst getan, Erz getragen, einen Pass überwunden oder im Kloster genächtigt?
- Wen kennt ihr hier: einen Mönch, eine Grenzsoldatin, einen Goldschmied, einen Bergmann oder eine Händlerfamilie?
- Was habt ihr in den Zhobergen verloren: einen Kameraden, einen Vorrat, ein Relikt oder einen Eid?
# Orte & Aufhänger
## Wichtige Orte
- **Omasch** – Hauptausbildungsstätte der Satrapiegarde.
- **Qadlus Mavari** – östlichste Ansiedlung Qadiras, Oasenort an der Goldstraße mit Lugalisimaru-Schrein.
- **Sonnenhügelkloster** – religiöses und organisatorisches Zentrum der Eleli unter einer Peri.
- **Gazbilah, Kharif, Naamat, Salav** – weitere Berg- und Randorte für Handel, Militär und Versorgung.
## Aufhänger
- Die Ausbildung in Omasch wird durch interne Intrigen, Grenzvorfälle oder fehlende Rekruten gestört.
- Qadlus Mavari braucht Schutz, weil die Goldstraße durch äußere oder übernatürliche Bedrohungen unter Druck gerät.
- Das Sonnenhügelkloster sendet Hilferufe wegen einer Gefahr, die zwischen Religion und Grenzsicherung liegt.
- Entlang des Weißen Passes verschwinden Händler, Soldaten oder Pilger.
# Zufallstabellen
## Terrain  
Steile Hänge, Pässe, alpine Wiesen, Felsgrate, Bergkämme, Hochplateaus, Nebeltäler, Geröllfelder, Oasenrand, schmale Handelsstraßen.
## Entdeckungen  
Verlassene Wachposten, Erzadern, alte Grenzmarkierungen, versteckte Klosterpfade, Drachenhöhlen, vergessene Schätze, Passheiligtümer, Lawinenreste.
## Begegnungen  
Bauern, Bergleute, Goldschmiede, Händler, Juweliere, Mönche, Soldaten, Waffenschmiede, Patrouillen, Greifen, Orks, Riesen, Feenwesen.
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
Die Region wird von Bauern, Bergleuten, Goldschmieden, Händlern, Juwelieren, Mönchen, Soldaten und Waffenschmieden bewohnt. Unter den nichtmenschlichen Gefahren und Nachbarn finden sich Chimären, Feenwesen, Greifen, Grottenschrate, Lamien, Oger, Orks, Riesen, rote Drachen und Zyklopen.
# Besonderheiten
Die Nördlichen Zhoberge leben von **Ausbildung, Kontrolle und Grenzblick** statt von Reichtum oder urbaner Vielfalt. Omasch und der Weiße Pass machen die Region militärisch relevant, Qadlus Mavari verknüpft sie mit der Goldstraße und religiöser Versorgung, und das Sonnenhügelkloster gibt ihr einen starken spirituellen Anker. Als regionale Regel passt hier besonders: **Wer die Pässe kontrolliert, kontrolliert nicht nur Handel, sondern auch die Stimmung vor dem Krieg.**

