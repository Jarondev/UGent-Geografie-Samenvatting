# Covariantie
Variantie: gekwadrateerde afwijking van een variabele tov gemiddelde
**Covariantie**: **product afwijkingen** van 2 variabelen tov gemiddelde
-> afhankelijk van eenheid/schaal

# Correlatiecoefficient
Gestandardiseerde maat voor **lineaire associatie tussen 2 variabelen** [-1, +1]
- -1: sterke **negatieve** correlatie
- 1: sterke **positieve** correlatie

Wordt beinvloed door **steekproefgrootte**
-> H<sub>0</sub> sneller verworpen bij grote steekproef
## Pearson's Correlatiecoefficient
### Assumpties
- Continue variabelen (interval, ratio)
- Normale verdeling
- **Geen lineair verband**
- **Geen uitschieters**
- Homoscedasticiteit
### Advies
1. Maak **scatterplot** om soort associatie na te gaan (kijk als lineair is)
2. **Voorzichtig** met associaties met oorzaak te linken
	- *Toeval/schijnverband* kan spelen
3. **Reproduceerbaarheid & transparantie**: wees duidelijk over genomen stappen
	-> door bv. doordacht om te gaan met uitschieters
4. Verschil kennen tussen significantie en sterke associatie
	-> bij grotere steekproef zijn kleine correlaties al significant
		-> minimale absolute significante waarde: **2/sqrt(n)**
5. r enkel interpreteren op **gekozen geaggregeerd niveau**
	-> *niet veralgemenen*

**Ecologische fout**: bestudeerde gegevens toepassen op onbestudeerde gebieden buiten aggregaat
## Spearman Correlatiecoefficient
### Assumpties
- **Ordinale** data
- Geen normale verdeling
- Niet lineair (bv. exponentieel)
### Stappenplan
1. 2 geordende sets maken voor elke variabele
2. Bereken **Pearson's correlatiecoefficient** voor geordende data
3. Kijk naar waarnemingen:
	1. Gelijke observaties: pearsons correlatiecoefficient met rangen als observaties
	2. Geen gelijke observaties: d<sub>i</sub> = verschil tussen rangen voor observatie i



