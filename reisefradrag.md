## Reisefradrag

### Modellparametre
- modell = gpt-4-0125-preview
- temperature = 0

### Kontekst
- Skatteloven § 6-44
- Finansdepartementets forskrift til skatteloven § 6-44
- Takseringsforskriften § 1-3-8
- Skatte-ABC R-8-1 til R-8-10

### Prompts
Vi tester flere ulike prompts. Ulike prompts gir ulike svar! For å legge inn lovtekst og tekst fra Skatte-ABC bruker vi koden {KONTEKST}. Når vi måter inn spørsmålene i modellen bytter vi ut {KONTEKST} med rettskildene. Merk at den første prompten nedenfor ikke har en slik {KONTEKST}. Da tester hva modellen klarer uten at den får norske rettskilder eksplisitt matet inn. 

- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt.
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST} Tenk trinn for trinn.
- Du er en norsk ekspert på skatterett som skal løse spørsmål om skatt. Vis alltid hvilket rettslig grunnlag du bygger på. Dersom du er i tvil, gjør nøye rede for hvorfor du er tvil. Legg vekt på å skrive et sammenhengende resonnement. Unngå å bruke punktlister. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse rettslige spørsmål om skatt. Bruk følgende metode. Formuler hva det rettslige spørsmålet dreier seg om. Finn det rettslige grunnlaget som regulerer spørsmålet. Finn alle argumenter som er relevante for spørsmålet. Vurder alle relevante argumenter og henvis til rettskilder der dette er relevant. Konkluder. Legg vekt på å skrive en sammenhengende tekst der du ikke bruker punktlister og nummereringer. Baser svaret på følgende kontekst: {KONTEKST}

### Tester
- [reisefradrag – uten kontekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/reisefradrag_uten_kontekst.md)
- [reisefradrag – lov og forskrifter](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/reisefradrag_lov_forskrift.md)
- [reisefradrag – lov og forskrifter + skatte-abc](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/reisefradrag_lov_forskrift_abc.md)

### Spørsmål med fasit
**Peder Ås har 35 km reisevei fra eget hjem til kontoret. I utgangspunktet arbeider han på kontoret 230 dager i løpet av året, men han har hatt 15 sykedager i 2023. Har Ås krav på reisefradrag og eventuelt hvor mye?**

Fasit: Spørsmålet om Ås har krav på reisefradrag reguleres av sktl. § 6-44 med supplerende forskriftsbestemmelser. 

Fradraget gis basert på reiseavstand og reisehyppighet, og er begrenset til den del av beløpet som overstiger 14 400, jf. § 6-44 (1). Av Finansdepartements forskrift til skatteloven § 6-44-1 følger det at reiseavstanden må være minst 2,5 kilometer hver vei for at man skal være berettiget til fradrag, og Ås oppfyller dette med sin reisevei på 35 km hver vei. 

Etter Finansdepartements forskrift § 6-44-3 (2) regnes det normalt med 230 arbeidsdager i et helt år og en reise tur-retur hver arbeidsdag. Fravær på grunn av sykdom, avspaseringer, permisjoner, yrkesreiser og lignende, skal trekkes fra i det totale antall arbeidsdager dersom fraværet utgjør mer enn 15 arbeidsdager i løpet av året, jf. samme sted. Siden Ås ikke har mer enn 15 dager med fravær på grunn av sykdom, skal det ikke gjøre noen fratrekk fra utgangspunktet på 230 dager. 

Det følger av Skattedirektoratets takseringsforskrift § 1-3-8 at fradrag settes til kr 1,70 per km, uansett reiselengde i året. Med 230 reisedager i året blir det til sammen 35x2x230x1,7 = kr. 27 370. Når vi trekker fra bunnfradraget på 14 400, gir det Ås et reisefradrag på kr. 12 970. 

**Peder Ås har 35 km reisevei fra eget hjem til kontoret med bil. Han har imidlertid også mulighet til å ta tog hvor reiseveien bare blir 30 km fordi toget går gjennom en tunnel. Med tog må han imidlertid gå 1,5 km (15 minutter) til og fra togstasjonene både ved hjemmet og ved arbeidsplassen. I utgangspunktet arbeider han på kontoret 230 dager i løpet av året, men han har hatt 15 sykedager i 2023. Har Ås krav på reisefradrag og eventuelt hvor mye?**

Fasit: Spørsmålet om Ås har krav på reisefradrag reguleres av sktl. § 6-44 med supplerende forskriftsbestemmelser. 

Fradraget gis basert på reiseavstand og reisehyppighet, og er begrenset til den del av beløpet som overstiger 14 400, jf. § 6-44 (1). Av Finansdepartements forskrift til skatteloven § 6-44-1 følger det at reiseavstanden må være minst 2,5 kilometer hver vei for at man skal være berettiget til fradrag, og Ås oppfyller dette med sin reisevei på over 30 km hver vei. 

Etter Finansdepartements forskrift til sktl. § 6-44-2 (1) beregnes reiseavstanden til korteste strekning av vei og distanse med rutegående transportmiddel bortsett fra fly, uavhengig av faktisk reisemåte. Ved reise med offentlig transport må man inkludere avstanden mellom hjem og arbeidsplass og stasjonene/holdeplassene, jf. Skatte-ABC R-8-4.4.1. Fordi Ås reisevei med tog blir på til sammen 36 km (30 km + 1,5x4) er den lengre enn avstanden med bil på 35 km, og derfor legges avstanden med bil til grunn. 

Etter Finansdepartements forskrift § 6-44-3 (2) regnes det normalt med 230 arbeidsdager i et helt år og en reise tur-retur hver arbeidsdag. Fravær på grunn av sykdom, avspaseringer, permisjoner, yrkesreiser og lignende, skal trekkes fra i det totale antall arbeidsdager dersom fraværet utgjør mer enn 15 arbeidsdager i løpet av året, jf. samme sted. Siden Ås ikke har mer enn 15 dager med fravær på grunn av sykdom, skal det ikke gjøre noen fratrekk fra utgangspunktet på 230 dager.  

Det følger av Skattedirektoratets takseringsforskrift § 1-3-8 at fradrag settes til kr 1,70 per km, uansett reiselengde i året. Med 230 reisedager i året blir det til sammen 36x2x230x1,7 = kr. 28 152. Når vi trekker fra bunnfradraget på 14 400, gir det Ås et reisefradrag på kr. 13 752. 

**Peder Ås har 35 km reisevei fra eget hjem til kontoret. I utgangspunktet arbeider han på kontoret 230 dager i løpet av året, men han har hatt 15 sykedager i 2023. I tillegg er det 20 dager han ikke har kjørt til jobben fordi han har sittet på med en kollega. Har Ås krav på reisefradrag og eventuelt hvor mye?**

Fasit: Spørsmålet om Ås har krav på reisefradrag reguleres av sktl. § 6-44 med supplerende forskriftsbestemmelser. 

Fradraget gis basert på reiseavstand og reisehyppighet, og er begrenset til den del av beløpet som overstiger 14 400, jf. § 6-44 (1). Av Finansdepartements forskrift til skatteloven § 6-44-1 (1) følger det at reiseavstanden må være minst 2,5 kilometer hver vei for at man skal være berettiget til fradrag, og Ås oppfyller dette med sin reisevei på 35 km hver vei. Av samme bestemmelse (5) følger det at det ikke påvirker retten til fradrag at flere reiser sammen i én bil. Ås kan derfor også få reisefradrag for de dagene han kjører med kollegaen.  

Etter Finansdepartements forskrift § 6-44-3 (2) regnes det normalt med 230 arbeidsdager i et helt år og en reise tur-retur hver arbeidsdag. Fravær på grunn av sykdom, avspaseringer, permisjoner, yrkesreiser og lignende, skal trekkes fra i det totale antall arbeidsdager dersom fraværet utgjør mer enn 15 arbeidsdager i løpet av året, jf. samme sted. Siden Ås ikke har mer enn 15 dager med fravær på grunn av sykdom, skal det ikke gjøre noen fratrekk fra utgangspunktet på 230 dager. 

Det følger av Skattedirektoratets takseringsforskrift § 1-3-8 at fradrag settes til kr 1,70 per km, uansett reiselengde i året. Med 230 reisedager i året blir det til sammen 35x2x230x1,7 = kr. 27 370. Når vi trekker fra bunnfradraget på 14 400, gir det Ås et reisefradrag på kr. 12 970. 



