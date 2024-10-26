# Transportsystemen
## Vraag
Zie hoofdstuk 5
## Nodes

Toegangspunt tot een transportnetwerk (bv. station)
-> **essentiele plaatsen** in netwerk

**Link**: infrastructuur (weg, sporen)
**Hub**: node met grote transportvolume
**Feeder**: node die gelinkt is met een hub
**Corridor**: serie van nodes (meestal lineair)

> [!Example] Voorbeeld
> Op *globale* schaal: (lucht)havens als nodes
> Op *regionale* schaal: steden
> Op *lokale* schaal: werk- en commerciele activiteiten
## Netwerk
*Structuur en organisatie* van **transportverbindingen**
### Types
````col
```col-md
flexGrow=1
===
#### Gecentraliseerd
- Enkel centrum heeft toegang tot alles

![[{CE476049-9CF3-412A-B0B3-8BD23F37439B}.png]]
```
```col-md
flexGrow=1
===
#### Gedecentraliseerd
- Centrum nog altijd centraal met sub-centra errond
![[{413911E4-0162-4859-A720-F78A5EF4F6EF}.png]]
```
```col-md
flexGrow=1
===
#### Gedistributeerd
- Geen duidelijk centrum

![[{F6EAC02B-3DBD-48DA-9BCA-39F4CF429BF8}.png]]
```
````
### Transportnetwerk
#### Types
**Centrifugaal**: meer *grid-patroon*
**Centripetaal**: meer centraliteit door *radiaal patroon*
**Gedistributeerd**: alle nodes zijn evenwaardig
**Point-to-point netwerk**: zelfde als gedistributeerd; geen centrum, nodes gaan naar omliggende

##### Hub and spoke netwerk (Gecentraliseerd)
- [p] Minder infrastructuur nodig
- [p] Frequentere verbindingen
- [p] Grotere capaciteit tussen netwerken 
- [c] Hogere reistijd door langere trajecten

#### Metcalfe's Law
Berekent **max nummer van unieke vebindingen die gemaakt kunnen worden in een netwerk**

### Netwerklengtes
````col
```col-md
flexGrow=1
===
- **Minimum netwerk** (A): meest simpele configuratie om een netwerk te vormen
- **Intermediate netwerk** (B/C): compromis tussen bereikbaarheid en kost
- **Compleet netwerk** (D): redundant netwerk met vaak overbodige verbindingen
```
```col-md
flexGrow=1
===
![[Pasted image 20241026200442.png|625]]
```
````
### Oorsprong
- **Random**: door willekeurige processen
- **Normaal**: elke node heeft even veel verbindingen (meestal ruimtelijk georganiseerd)
- **Small-world**: veel verbindingen met nabije nodes
- **Scale-free**: hubs met veel verbindingen (hub and spoke-achtig)