## Kwadrantanalyse
	= Methode om puntpatronen te onderzoeken
**Vraag**: zijn punten uniform verspreid of geconcentreerd?
Puntpatronen **verdelen in kwadranten** (rooster)
-> **grootte belangrijk** (MAUP)

Gegevens moeilijk op zo klein mogelijk schaal te zetten: **small numbers problem**
-> leidt tot insignificantie door te veel lege data

**Variance Mean Ratio** (*VMR*): kijken naar concentratie puntpatroon
- VMR < 1: uniform (gelijke verspreiding)
- VMR > 1: geconcentreerd
- VMR = 0: random

### Statistische Test
1. Hypothese: puntpatroon is random
2. Bereken toetsstatistiek 𝜒2
3. Vergelijk berekende waarde met kritische waarde met m-1 vrijheidsgraden

Bij 6x6 rooster (36 kwadranten): **normale verdeling en z-scores gebruiken**

## Ruimtelijke Aspecten Regressieanalyse
**Ruimtelijke Autocorrelatie**: relevantie waarde punt ivm omliggende punten
-> kan negatief of positief zijn ([-1, 1])

> ![[Safari _ 18-12-2024_0342PM@2x.png|400]]

Geschonden assumpties:
1. Homoscedasticiteit
2. Onafhankelijkheid
3. Normaliteit

**Probleem** voor regressieanalyse: data afhankelijk van ruimte
Maar: 
- Soms **geinteresseerd in ruimtelijk gecorreleerde residuen** om nieuwe hypothesen te maken
- Kan wijzen op *ruimtelijke relaties variabelen*, of *verschil in opmetingen* afh. van persoon

Oplossing: lokale regressiecoëfficienten

### Plan
1. Bouw regressiemodel op
2. Bereken Moran's I om **autocorrelatie** vast te stellen
3. Visualiseer residuen op kaart
4. Indien autocorrelatie, gebruik **ruimtelijke regressietechnieken**
	- **Spatial lag** model voor *afhankelijkheid in variabelen*
		-> er wordt niet dieper ingegaan op relaties, *corrigeert enkel*
	- **Spatial error** model voor *afhankelijkheid residu*
	- **Expansiemethode** om lokale variaties en trends te modelleren dmv coordinaten of hogere-orde termen
		-> laat toe dat relaties tussen variabelen in ruimte varieren

**Globale regressiemodellen**: helling en intercept **geldig voor alle observaties**
**Lokaal**: helling en intercept in *functie van andere variabelen*

**Geografisch gewogen regressie**: lokale variaties in ruimtelijke relaties analyseren door lokale regressievergelijkingen te maken voor elke locatie met gewichten 