---
type: region
biome:
  - "[[Ebenen & Steppen]]"
  - "[[Quellen]]"
  - "[[Dschungel]]"
  - "[[Hügel]]"
  - "[[Karawanenwege & Handelsrouten]]"
  - "[[Fluss- und Wadi-Täler]]"
banner_image: https://www.mckinnonfilms.com/wp-content/uploads/2001/04/Jazan-Area-and-the-Tihama-Plains-Potential-for-Agricultural-Investment-001.jpg
---
# Regionsbeschreibung
## Kurzbeschreibung  
Die Pareschebene ist Qadiras große Gras- und Handelsregion, Heimat der Hauptstadt Katheer, der Goldstraße und einer dicht besiedelten, halbnomadischen Kultur zwischen Hirtenleben, Stadtwirtschaft und Grenzkrieg. Sie wirkt offen und wohlgeordnet, ist aber von Taldor, Steuern, Räubereien und alten Scharmützeln dauerhaft geprägt.
## Lage & Kontext  
Die Ebene liegt um Katheer und die großen Handelsstädte Al-Varisch, Avilan, Delenah und Demirah. Im Westen und Süden verbindet sie sich mit den weiteren qadirischen Binnen- und Küstenräumen, im Norden wird sie von der Rivalität mit Taldor und dem Grenzwald beeinflusst. Als Herz des Reiches ist sie politisch, wirtschaftlich und infrastrukturell das Zentrum Qadiras.
## Impressionen  
**Immer:** Weite Grasflächen, Wind über der Ebene, weiße Straßen und Banner, Karawanenverkehr, Herden, Pferdehufe, die Nähe einer großen Stadt auch dort, wo die Landschaft offen wirkt.  
**Frühling:** Frische Weiden, lebhafte Märkte, neugeborene Tiere, viel Bewegung auf den Handelswegen, stabile Reisezeit.  
**Sommer:** Warme Ebenen, staubige Straßen, starke Sonneneinstrahlung, dichtes Leben in Städten und Herdenlagern, Karawanen unter strenger Bewachung.  
**Herbst:** Reife Herden, Ernte, diplomatische Reisen, gute Sicht, erhöhte Aktivität auf der Goldstraße.  
**Winter:** Kältere Nächte, kräftige Winde, langsamere Handelsbewegung, mehr Konzentration auf Städte, Lager und Herbergen.
## Das prägende Element  
Das prägende Element ist die **Hauptader des Reiches**: die Pareschebene verbindet Landwirtschaft, Hauptstadt, Luxus und Handel mit einer permanenten Grenzspannung nach Norden. Hier zeigt sich Qadira als Reich der Straßen, Städte und Herden.
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
- Warum will ein so großer Teil der Bevölkerung hier den Krieg mit Taldor beinahe herbeisehnen?
- Was schützt die Goldstraße wirklich: Magie, Militär oder die Wirtschaft des Reiches?
- Welche alten Narben und Fallen liegen im Grenzwald und an den Verkehrsachsen der Ebene?
## Fragen an die Figuren
- Wer von euch ist mit Katheer, den Herbergen der Goldstraße oder den Handelsstädten aufgewachsen?
- Wen kennt ihr hier: einen Händler, einen Falkner, eine Rechtsgelehrte, einen Hirten oder einen Karawanenführer?
- Was habt ihr auf der Pareschebene verloren: ein Geschäft, ein Pferd, eine Familie, ein Dokument oder einen Anspruch?
# Orte & Aufhänger
## Wichtige Orte
- **Katheer** – Hauptstadt Qadiras am Paschman.
- **Al-Varisch, Avilan, Delenah, Demirah** – große Handelsstädte mit fast städtischer Dichte wie die Hauptstadt.
- **Goldstraße** – Handelsnetz mit magischen Brunnen und kaiserlicher Kontrolle.
- **Grenzwald / Jalrune** – scharfe Grenzlinie und Scharmützelschauplatz gegen Taldor.
- **Sarayküste** – Küstenland mit Hafenorten, Piraten und Schakalwere-Verstecken.
- **Turm des Windes** – rätselhafter Turm auf der grasbewachsenen Steppe.
## Aufhänger
- Eine Karawane auf der Goldstraße wird durch Steuern, Räuber oder politische Intrigen bedroht.
- Im Grenzwald verschwinden Späher oder werden alte Fallen reaktiviert.
- Katheer braucht diskrete Hilfe bei einem inneren Machtkampf.
- An der Sarayküste bauen Piraten oder Schakalwere eine neue Gefahr auf.
- Der Turm des Windes scheint auf etwas zu reagieren, das mit der gesamten Ebene zu tun hat.
# Zufallstabellen
## Terrain  
Grasebenen, bewässerte Felder, Herdenpfade, Handelsstraßen, Grenzwald, Flussläufe, Küstenklippen, offene Hügel, befestigte Herbergen, Stadtviertel.
## Entdeckungen  
Magische Brunnen, alte Scharmützelfelder, zurückgelassene Banner, Grenzfallen, versteckte Herdenlager, Handelszeichen, Ruinen an der Küste, verlassene Späherposten.
## Begegnungen  
Bauern, Hirten, Händler, Kleriker, Schreiber, Alchemisten, Anwälte, Ärzte, Falkner, Räuber, Stadtbewohner, Karawanenwächter, Grenzspäher, Piraten.
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
Die Pareschebene wird von halbnomadischen Stämmen, Hirten, Händlern und Stadtbewohnern geprägt, die stark zwischen Land und Stadt vermittelt leben. Dazu kommen Elefanten, Herdentiere, Kamele, Kobras, Löwen, Paviane, Pferde, Riesenameisen, Schakalwere und Zebras.
# Besonderheiten
Die Pareschebene ist Qadiras **politisches und wirtschaftliches Zentrum** und zugleich seine emotionalste Grenzregion, weil hier der Konflikt mit Taldor am stärksten gespürt wird. Katheer und die Goldstraße machen sie reich und sichtbar, der Grenzwald macht sie narbig und angespannt, und die Sarayküste bringt zusätzlich Küstengefahren ins Spiel. Als regionale Regel passt hier besonders: **Wer hier reisen, handeln oder herrschen will, muss immer gleichzeitig an Grenze, Steuern und Loyalität denken.**

