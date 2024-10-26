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

Aantal nodes = *order*
Aantal links = *size*

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
#### Classificaties
##### Op basis van Centraliteit
**Centrifugaal**: meer *grid-patroon*
**Centripetaal**: meer centraliteit door *radiaal patroon*
##### Op  basis van verbindingen
**Point-to-point netwerk**: zelfde als gedistributeerd; geen centrum, nodes gaan naar omliggende

**Hub and spoke netwerk** (Gecentraliseerd)
- [p] Minder infrastructuur nodig
- [p] Frequentere verbindingen
- [p] Grotere capaciteit tussen netwerken 
- [c] Hogere reistijd door langere trajecten
##### Op basis van aantal verbindingen
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
##### Op basis van structuur
**Random**: door willekeurige processen
**Normaal**: elke node heeft even veel verbindingen (meestal ruimtelijk georganiseerd)
**Small-world**: veel verbindingen met nabije nodes
**Scale-free**: hubs met veel verbindingen (hub and spoke-achtig)
#### Metcalfe's Law
Berekent **max nummer van unieke vebindingen die gemaakt kunnen worden in een netwerk**
#### Redenen voor (geen) verbindingen
- Initiele bouwkost
- Onderhoudskost
- Nodes met prioriteit (hubs)
- Max. toegankelijkheid tot andere nodes
- Kortste afstand van het netwerk
- Kortste afstand tussen alle locaties (traveling salesman)

#### Transportkost
**Hogere kosten** op verbindingen tussen **verafgelegen nodes**
-> hogere algemene kost in gedecentraliseerd netwerk

#### Kenmerken
- **Coevolutie**: vergelijkbare of uiteenlopende ontwikkelingen
	- Door *nabijheid* of *economische* ontwikkelingen
	- Grotere *diversiteit in kerngebieden* dan afgelegen gebieden
- **Complementariteit**: prioriteit hub afhankelijk van specialisatie, functie en schaal
- **Interoperabiliteit, inter-modal shifts**: compatibiliteit tussen middelen
	- Bv. maritiem naar wegennetwerk:
		- van *scale-free structuur naar normale structuur*
- **Kwetsbaarheid**: hoe veranderingen in een netwerk een ander beinvloeden
	- Op lokaal of globaal level
	- Belangrijk om *redundantie* in gedachten te houden (voor bv. natuurrampen)
## In Ruimte
### Types
- **Duidelijk gedefineerd**: 
	- Ruimte heeft *1 specifiek doel*
	- Heeft een *eigenaar*
- **Vaag gedefineerd**:
	- *Niet exclusief* voor transportmiddel
	- *Geen* specifieke *eigenaar*
- **Zonder definitie**: ruimte is niet duidelijk gedefineerd

> [!Example] Voorbeeld
> ![[{2EE03AAD-E8B0-4CAB-9F83-30A1102E9804}.png]]
### Fysieke beperkingen
**Absolute barriere**: geografie zondert mode van transport volledig uit
	-> bv. auto's op zee
**Relatieve barriere**: geografie bemoeilijkt mode van transport
	-> bv. wegen door bergen
#### Factoren
- **Topografie** (bergen, kust,...)
- **Hydrologie** (water is bonus voor maritiem, malus voor trein & auto)
- **Klimaat** (jet stream voor vliegtuigen, natuurrampen..)
## Netwerkanalyse
### Sociale Netwerk Analyse (SNA)
Sociale structuur analyseren door te kijken naar patronen in flows van netwerken
#### Op netwerk niveau
Analyse **dichtheid van algemeen netwerk**
-> *bereikbaarheid tussen alle punten* op een netwerk
Hangt af van grootte netwerk
#### Op node niveau
**Centraliteit** van de individuele node
-> hoe belangrijk is knooppunt?

**Gerichte vs ongerichte** verbinding: stroomt verkeer in 1 richting of beide?
**Paden**: sequentie punten in een netwerk
-> kortste/snelste/makkelijkste pad hangt af van beschikbare verbindingen tussen nodes
##### Centraliteitsgraad
Hoeveel verbindingen de node heeft met omliggende nodes
-> toont **hoogste vermogen** aan in netwerk

Bij gerichte verbindingen: kijken naar **indegree vs outdegree**
-> hoeveel verbindingen komen toe,  hoeveel vertrekken
##### Nabijheid
Toont **afhankelijkheid** van andere nodes
Ook indicator voor *toegankelijkheid*

Meet *gemiddelde afstand van 1 node naar alle andere nodes* in een netwerk
##### Tussenheid
Analyseert **positie** van een node in een netwerk
Indicator voor *controle*

Meet *hoeveel keer de node op het kortste pad ligt*
#### Clusters
Belang **sub-netwerken**
-> nodes die *meer verbonden zijn met elkaar* dan buiten cluster
### Concentratieindex
	= Om concentratie van een netwerk te meten
**Concentratie ratio**: gemeenschappelijk aandeel x-nodes of verbindingen met hoogte hoeveelheid stromen
-> kijkt naar meest significante knooppunten met *overlappende netwerken*

**Herfindahl-Hirschman index**: som van het kwadraat van alle aandeelhouders
-> *laag HHI: meer competitief*

**Gini-index** (GI): waarde tussen 0 en 1 die concentratie aangeeft

**Network concentration index** (NCI): verhouding tussen GI en max. GI