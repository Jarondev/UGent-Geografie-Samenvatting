# Regressieanalyse
Beschrijft **lineaire relatie** tussen *afhankelijke en onafhankelijke continue variabele* met een model
ŷ = a + bx
-> y: voorspelde waarde, x: geobserveerde waarde, a: intercept (punt op y as), b: helling
**residu**: verschil op y-as tussen voorspelling en variabele

Significant is niet altijd zinvol! (F-toets)
## Regressie voor Bivariate Data
Standaard **verticale afstand**
- Fouten alleen in y-richting
-> euclische afstand voor meetfouten/symmetrische data

Som alle residuen = 0
## Eigenschap
Verdeelt variantie in Y op in elke observatie voor:
- **Verklaarde variantie** (berekend door model) = SSR
- **Residuele variantie** (+ residu) = SSE

r<sup>2</sup> geeft aan welk **percentage van de totale variantie verklaard wordt** door regressiemodel
-> r<sup>2</sup> = **0.8 wijst op 80% correlatie** met X

**Significantietest**: kijken als regressiemodel significant deel van variantie in y verklaart
-> **F-toets** om te verhouding verklaarde variantie met residuele variantie te vergelijken
- Grote F-waarde duidt op betere verklaring variantie in Y
**P-waarde** berekend op basis van F-toets om te kijken als model significant is
-> p < 0.05: model is significant

**Standaardfout schatting** = standaardafwijking residu
-> kijken nauwkeurigheid model

**T-toets** om te kijken als onafhankelijke variabele een significant effect heeft

## Assumpties (Enkelvoudige Regressie)
1. **Lineariteit**: relatie is lineair voor populatie 
2. **Homoscedasticiteit**: residu met gemiddelde 0 en constante variatie
3. **Onafhankelijkheid**: *onafhankelijke residuen*
4. **Normaliteit**: normale verdeling van fouten