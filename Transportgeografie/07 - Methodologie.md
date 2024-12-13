# Geaggregeerde benadering: 4 step modelling approach
	= Op basis van flows/stromen, afhankelijk van doelstelling
Kijken hoe wijzigingen infrastructuur gehele systeem beinvloeden

Voordelen: makkelijk toe te passen, geschikt voor wijzigingen aan netwerk (circulatieplan)
Nadelen: **Simpson paradox**
- Door zaken te aggregeren krijg je potentiele fouten (minder detail)
Stap 0: zones defineren
## 1. Trip Generatie
Kijken hoeveel verplaatsingen die in en uit een zone gaan
Verplaatsingen analyseren aan de hand van regressieanalyse

Onafhankelijke variabelen X tellen op tot Y
-> kijken welke rol ze spelen
	-> bv. inwoners in een regio: als er niemand woont: geen verplaatsing
	-> hoeveel jobs, bedrijven...
**Regressievergelijking toont effect X op Y**

> [!Example] Voorbeeld
> Y = 0.0649 X<sub>1</sub> – 0.0034 X<sub>2</sub> + 0.0066 X<sub>3</sub> + 0.9489 X<sub>4</sub>
> 
> Y = totale auto trips per gezin per 24h
> X<sub>1</sub> = grootte gezin
> X<sub>2</sub> = bevolkingsdichtheid woonwijk
> X<sub>3</sub> = totale gezinsinkomen
> X<sub>4</sub> = beschikbare autos per gezin
> 
> X <sub>1,2,3</sub> zijn laag, lage impact
> X<sub>4</sub> hoog, hoge impact

## 2. Trip Distributie
Kijken hoeveel verplaatsingen tussen 2 zones
### Modeltypes
- Beperkt (constraint): O of D gekend
- Niet-beperkt: niks gekend
	- Productiebeperkt
		- Totaal is gekend, aantal huishoudens
		- Aantal winkels niet gekend
		-> 3x schalingsniveau toepassen
	- Aantrekkingsbeperkt
- Dubbel beperkt: O & D gekend

Beperkt is interessant, makkelijk om analyses en vaststellingen te maken

## 3. Modale uitsplitsing
	= Analyse om te voorspellen welke modus gebruikt zal worden
**Frequentie berekenen**
Afhankelijk van: 
- Karakteristieken individu (leeftijd, inkomen, autobezit)
- Karakteristieken trip (afstand)
- Karakteristieken modus (reistijd, kost, comfort)

## 4. Route Toewijzing
Via autosnelweg, via hoofdwagen, binnenbaantjes...
- **Stochastisch effect**: willekeurige routes adhv congestie
- Congestie

# Gedisaggregeerde Modelling Approach
Op **individueel niveau**, data wordt niet geaggregeerd
Zelfde stappen + **wanneer** trip is gemaakt

Trip/tour models

## Activiteitsgebaseerde Modelling Approach
Verplaatsingen worden afgeleid uit activiteiten persoon
- Woon-werk
- Boodschappen
- Eten
