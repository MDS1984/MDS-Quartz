---
type: region
biome:
  - "[[Gebirge]]"
  - "[[Hügel]]"
  - "[[Canyons & Schluchten]]"
  - "[[Quellen]]"
  - "[[Verlassene Ruinen & Steinwüsten]]"
banner_image: https://peakvisor.com/photo/SD/Saudi-Arabia-Soudah-Mountains.jpg
---
# Regionsbeschreibung
## Kurzbeschreibung  
Die Südlichen Zhoberge sind eine zerklüftete, wenig bereiste Bergregion voller gefährlicher Kreaturen, Schmugglerpfade, alter Ruinen und einzelner abgelegener Siedlungen. Zwischen Vulkanen, Klöstern, verborgenen Festungen und alpinen Tälern mischen sich Mystik, Gesetzlosigkeit und rohe Berggewalt.
## Lage & Kontext  
Der längste zusammenhängende Teil der Zhoberge liegt südlich des Paschman und zieht sich bis zur Küste weiter. Das Gelände ist so schwierig, dass Transport und Reise mühsam bleiben, wodurch die Region klein besiedelt und schwer kontrollierbar ist. Genau diese Abgeschiedenheit macht sie zu einem Rückzugsraum für Schmuggler, verbannte Gruppen und viele der gefährlichsten Kreaturen Qadiras.
## Impressionen  
**Immer:** Scharfe Felskämme, kalte Bergluft, Schwefelhauch, entfernte Dröhnlaute aus Vulkanen, enge Pfade, Schatten in Schluchten, das Gefühl von Höhe, Einsamkeit und Gefahr.  
**Frühling:** Schmelzwasser, instabile Hänge, lebendige Bergwiesen in kurzen Fenstern, mehr Bewegung von Hirten, Jägern und Reisenden.  
**Sommer:** Klare Sicht, karge Höhen, starke Sonne auf Stein, trockene Wege, mehr Schmuggel und Fernblick über die Täler.  
**Herbst:** Windige Pässe, erste Kälte, rauchige Horizonte, zunehmende Gefahr durch Ausbrüche, Steinschläge und Tierbewegungen.  
**Winter:** Schnee, Eis, abgeschlossene Täler, isolierte Siedlungen, heiße Quellen als kostbare Zuflucht und besonders harte Reisebedingungen.
## Das prägende Element  
Das prägende Element ist die **gefährliche Bergwildnis mit vulkanischem Herz**. Die Region ist kein bequemer Passraum, sondern eine Zone, in der Naturgewalt, alte Geheimnisse und soziale Randfiguren nebeneinander existieren.
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
- Warum sind die Südlichen Zhoberge so viel weniger kontrolliert als die übrigen Grenzräume?
- Was verbindet die alten Mythen der Zornigen Brüder mit den Vulkanen Zhobl und Zhonar wirklich?
- Welche Mächte schützen oder verbergen die verborgenen Festungen, heißen Quellen und abgelegenen Ortschaften?
## Fragen an die Figuren
- Wer von euch hat in den Bergen gejagt, geschmuggelt, geschürft oder eine der abgelegenen Siedlungen besucht?
- Wen kennt ihr hier: einen Töpfer, eine Schmugglerin, einen Mystiker, eine Oreadin oder einen Ork-Söldner?
- Was habt ihr in den Südlichen Zhobergen verloren: ein Versteck, eine Karte, einen Rivalen, ein Lager oder einen Eid?
# Orte & Aufhänger
## Wichtige Orte
- **Gurat** – kleine befestigte Stadt mit dem rätselhaften Sprachrohr, Zentrum für Mystiker und Teppichknüpfer.
- **Kristallklippe** – abgelegener Ort unter Illusionsschutz, bewohnt von Oreaden und Pyriern.
- **Blutfels** – verborgene Festung und düsteres Kult-Relikt mit Lamaschtu-Bezug.
- **Quellen des Vergessen** – Schwefelquellen mit gefährlicher, erinnerungsraubender Wirkung.
- **Schadun** – einstige Stadt, jetzt von Gnollen heimgesucht.
- **Zhobl und Zhonar** – die Zornigen Brüder, Vulkanberge und mythische Schicksalsorte.
## Aufhänger
- Ein Schmuggelpfad führt durch ein Gebiet, in dem sich Vulkangefahr und Gesetzlosigkeit überschneiden.
- Das Sprachrohr von Gurat braucht einen Boten, Beobachter oder Hüter für eine rätselhafte Prophezeiung.
- Die Quellen des Vergessens ziehen Reisende an, die ihre Vergangenheit oder einen Fluch loswerden wollen.
- In Blutfels oder Schadun regen sich alte, brutale Mächte erneut.
- Ein Ausbruch von Zhobl oder Zhonar droht eine ganze Route, Siedlung oder Kultstätte zu verschlingen.
# Zufallstabellen
## Terrain  
Zerklüftete Berge, Vulkanhänge, Lavageröll, enge Pässe, Hochplateaus, Felsklippen, Schwefelquellen, Schneefelder, verborgene Schluchten, Felsnester.
## Entdeckungen  
Verlassene Schmugglerlager, alte Kultsymbole, Illusionsmarkierungen, heiße Quellen, versteckte Pfade, untergegangene Siedlungen, Drachenkrallen, Prophezeiungsteppiche, kultische Inschriften.
## Begegnungen  
Mystiker, Philosophen, Astrologen, Teppichknüpfer, Schmuggler, Orks, Gnolle, Oreaden, Pyrier, Bergjäger, Vulkanpriester, Riesen, Drachen.
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
Die Region ist dünn besiedelt, aber sehr charaktervoll: Mystiker, Philosophen, Astrologen und Teppichknüpfer leben neben Schmugglern, Bergarbeitern, Oreaden, Pyriern und Orks. Unter den nichtmenschlichen Bewohnern und Bedrohungen finden sich Aasimare, Blaue Drachen, Couatls, Donnervögel, Elementargeister, Gnolle, Gorgonen, Oger, Orks, Pyrier, Rakschasa, Riesen, Rieseneidechsen, Rochs, Rote Drachen, Schreckenslöwen und Sphingen.
# Besonderheiten
Die Südlichen Zhoberge sind eine Region der **Gefahr, der Isolation und der verborgenen Bedeutungen**. Gurat bringt Prophezeiung und Bildung, Kristallklippe Illusion und Exotik, Blutfels und die Quellen des Vergessens geben der Region einen dunklen, beinahe tabuierten Kern. Als regionale Regel passt hier besonders: **Was in den Südlichen Zhobergen verborgen ist, bleibt selten harmlos.**

