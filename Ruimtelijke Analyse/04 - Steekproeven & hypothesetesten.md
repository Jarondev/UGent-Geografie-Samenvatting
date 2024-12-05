# Steekproef
## Types
- **Random steekproef**
	Populatie selecteren uit *pure willekeur*
	Voor informatie over populatie zonder informatie over subgroepen
- **Systematische steekproef**
	*Systematisch aanpassen selectie* om resultaten gelijk te houden (bv. mannen & vrouwen)
- **Proportionele gestratificeerde steekproef**
	Steekproef moet *even veel observaties uit beide groepen* hebben
- **Disproportionele gestratificeerde steekproef**
	Als kleine subgroep populatie klein is, die *oversamplen door verhouding*
	bv. er zijn minder mannen dan vrouwen
## Ruimtelijke steekproeven
Om te kijken hoe grootte zich door ruimte uitspeelt
- **Random**
	*Random coordinaten* binnen volledige ruimte selecteren
- **Systematisch**
	Altijd op zelfde plek in zone na random in eerste zone
- **Gestratificeerd**
	In elke zone op willekeurige plek

**Composite sample**: combineren meerdere types steekproeven

# Steekproefgroottes
W = betrouwbaarheidsinterval van gemiddelde
-> /2 in formules


***Kwaliteitscheck***:
- Kijken naar invultijd, antwoordgedrag
- Vragen die zelfde antwoord zouden moeten geven

# Betrouwbaarheidsintervallen
***Centrale limietstelling***: gemiddelde van genoeg steekproeven geeft uiteindelijk normale verdeling
## Voor het gemiddelde
Gemiddelde steekproef nooit gelijk aan gemiddelde populatie
-> **betrouwbaarheidsinterval** nodig: *waarde ligt binnen zoveel %* van geschat gemiddelde

***Bij kleinere n: grotere interval***

Hoe zekerder uitspraak: grotere interval (99% betrouwbaarheidsinterval groter dan 95%)
## Bij een kleine steekproef (n<30)
**t-verdeling** gebruiken: betrouwbaarheid wordt breder met zelfde interval
	-> t-distributie meer gespreid dus meer oppervlak gebruikt voor zelfde interval
**t-tabel**: met df (*vrijheidsgraden*)
## Tussen 2 gemiddelden
Om steekproeven met elkaar te vergelijken
## Voor proporties
Voor proporties: bv 20/45 inwoners verhuisd
## Ruimtelijke data en gevolgen van onafhankelijkehid
***Eerste wet van geografie***: dingen dichtbij elkaar hebben meer gelijkenis
### Gevolg
- Niet representatieve steekproef
- Statistische onzekerheid
- Ruimtelijke autocorrelatie
### Oplossingen
- Verhoog grootte steekproef
- Gebruik alternatieve methodes
- Pas analsye aan
# Hypothese Testen
Significantie: meten en bepalen groepen populatie op basis van statistische test
Relevantie: kijken als verschil significantie relevant is

Hypothese is niet juist/fout -> *kwaliteit sterkte hypothese*
## Stappenplan
1. Stel **nulhypothese** H<sub>0</sub>
2. Opstellen **alternatieve hypothese** H<sub>A</sub>
	- (meestal) verwerpen nulhypothese
3. Bepaal significantieniveau α
	- (meestal) 0.05
4. Kies gepaste **statistische test en toetsstatistiek**
	- centrale limiet stelling: n>30
5. Bepaal **kritische waarde**
	- punt waarop hypothese verworpen/aanvaard wordt
6. **Vergelijk toetsstatistiek met kritische waarde** en verwerp/aanvaard H<sub>0</sub>
7. Bepaal p-waarde geassocieerd met extreme waarden
	- kans op waarde die extremer is dan toetsstatistiek
	- -p-waarde < α -> H<sub>0</sub> verwerpen

## Significantieniveau
**Type 1-fout**: ware H verwerpen (alpha error)
**Type 2-fout**: onware H aanvaarden (beta error)

Significantieniveau bepaalt *voorzichtigheid bij trekken conclusies*
-> minder kans op type 1 fout

## Bij kleine steekproef
### Voor gemiddelde
T-verdeling met n-1 vrijheidsgraden
### Voor proporties
T-test voor *verdeling steekproefproporties*

## 2 Steekproeven
### Gepaarde & Ongepaarde T-Test
- Gepaard: gegevens zijn **gerelateerd**
	Voor- en na behandeling
- Ongepaard: **niet-gerelateerde** gegevens
	verschil 2 verschillende groepen: bv controle en experimentele groep
### Effectgrootte
Meten grootte verschil tussen gemiddelde waarden van 2 groepen
-> hoe groter Cohen's d -> groter verschil

### Homo- of heteroscedasticiteit
Gelijke vs ongelijke spreiding resultaten
-> als varianties steekproeven niet gelijk zijn