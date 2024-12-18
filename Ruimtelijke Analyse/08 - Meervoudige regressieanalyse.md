# Meervoudige Regressieanalyse
Regressieanalyse in 3D

Zelfde assumpties + **Geen multicolinieariteit**: variabelen mogen *onderling niet gecorreleerd* zijn
-> **correlatiematrix** gebruiken om te kijken wat mag wegvallen
-> berekening **tolerantie**: proportie variantie in onafhankelijke variabele die niet verklaard wordt door andere variabelen
-> **Variance Inflation Factor** (*VIF*):  omgekeerde tolerantie
	-> kijkt hoeveel variantie wordt vergroot door multicolineariteit
	-> VIF > 5: mogelijke multicolineariteit

Opties bij multicolineariteit:
1. Laten zoals het is
	Stel: je wil **uitkomst voorspellen**, maakt niet uit hoe (black box)
		-> multicolineariteit wordt *irrelevant*
	Stel: je wil **uitkomst verklaren** (wat binnen black box gebeurt)
		-> multicolineariteit *belangrijk*
1. Variabele verwijderen
2. Nieuwe composiet van sterk gecorreleerde variabelen maken

## Gecorrigeerde R<sup>2</sup>
**Bij weinig observaties** t.o.v. aantal variabelen

Belangrijk **voldoende observaties** te hebben **tov aantal onafhankelijke variabelen**
## Misspecifcation Error
Wanneer *onafhankelijke variabelen die afhankelijke variabelen beinvloeden* **worden weggelaten uit de vergelijking**
-> overgebleven variabele neemt zowel eigen als 'vergeten' op zich
## Dummyvariabelen
**Categorisch onafhankelijke variabelen**
-> om privacy en oncomfortabiliteit te vermijden
- Voorbeeld: inkomensklassen, locaties

Binair: 0 of 1 (binnen categorie of niet)
Aantal: k-1
-> laatste variabele kan achterhaald worden adhv de andere (indien alle andere 0 zijn is laatste 1)

## Selecteren Variabelen
Adhv **inzicht in onderliggende processen** en bijhorende hypothesen
### Strategieën
1. **Backward Selection** (elimineren)
	-> variabelen verwijderen die minst aan r<sup>2</sup> bijdragen tot daling significant wordt
2. **Forward Selection** (correlatie)
	- Bepalen correlatie onafhankelijke en afhankelijke variabelen
	- Regressie met variabele met **hoogste correlatie**
	- Extra variabelen met significante correlatie toevoegen tot weinig meerwaarde
3. **Stepwise Regression** (hybride)
	- Combinatie forward en backward
		-> eerst forward dan backward
