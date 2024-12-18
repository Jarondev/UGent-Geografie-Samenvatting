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