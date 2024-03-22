## Avskrivninger

### Modellparametre
- modell = gpt-4-0125-preview
- temperature = 0

### Kontekst
- skatteloven kap. 6 (hele)
- skatteloven kap. 14 (hele)
- Skatte-ABC V-3 (Vedlikehold)
- Skatte-ABC D (Driftsmiddel)

### Prompts
Vi tester flere ulike prompts. Ulike prompts gir ulike svar! For å legge inn lovtekst og tekst fra Skatte-ABC bruker vi koden {KONTEKST}. Når vi måter inn spørsmålene i modellen bytter vi ut {KONTEKST} med rettskildene. Merk at den første prompten nedenfor ikke har en slik {KONTEKST}. Da tester hva modellen klarer uten at den får norske rettskilder eksplisitt matet inn. 

- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt.
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST} Tenk trinn for trinn.
- Du er en norsk ekspert på skatterett som skal løse spørsmål om skatt. Vis alltid hvilket rettslig grunnlag du bygger på. Dersom du er i tvil, gjør nøye rede for hvorfor du er tvil. Legg vekt på å skrive et sammenhengende resonnement. Unngå å bruke punktlister. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse rettslige spørsmål om skatt. Bruk følgende metode. Formuler hva det rettslige spørsmålet dreier seg om. Finn det rettslige grunnlaget som regulerer spørsmålet. Finn alle argumenter som er relevante for spørsmålet. Vurder alle relevante argumenter og henvis til rettskilder der dette er relevant. Konkluder. Legg vekt på å skrive en sammenhengende tekst der du ikke bruker punktlister og nummereringer. Baser svaret på følgende kontekst: {KONTEKST}

### Tester
Vi har utviklet to sett av spørsmål: spørsmål om avskrivninger for drosjebiler og spørsmål om avskrivninger for kontoreiendom. De to settene er hver for seg bygd opp slik at spørsmålene etter hvert blir mer kompliserte. 

Vi tester også kvaliteten på svarene varierer med hvor mye kontekst (rettskilder) vi mater inn. Her har vi brukt seks forskjellige alternativer: 1) ingen kontekst, 2) bare lovetekst, 3) lovtekst + Skatte-ABC, 4) lovtekst pluss et eksempel på hvordan avskrivninger skal regnes ut, 5) knappp lovtekst og 6) knapp lovtekst + eksempel.

#### Drosjebil
- [drosjebil – uten kontekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_drosjebil_uten_kontekst.md)
- [drosjebil – bare lovtekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_drosjebil_bare_lovtekst.md)
- [drosjebil – med lovtekst + Skatte-ABC](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_drosjebil_lov_abc.md)
- [drosjebil – med lovtekst + eksempel på utregning](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_drosjebil_lov_eksempel.md)
- [drosjebil - knapp lovtekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_drosjebil_knapp_lovtekst.md)
- [drosjebil – knapp lovtekst + eksempel](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_drosjebil_knapp_lovtekst_eksempel.md)

#### Kontoreiendom
- [kontoreiendom – uten kontekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_kontoreiendom_uten_kontekst.md)
- [kontoreiendom – bare lovtekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_kontoreiendom_bare_lovtekst.md)
- [kontoreiendom – med lovtekst + Skatte-ABC](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_kontoreiendom_lov_abc.md)
- [kontoreiendom – med lovtekst + eksempel på utregning](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_kontoreiendom_lov_eksempel.md)
- [kontoreiendom – knapp lovtekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_kontoreiendom_knapp_lovtekst.md)
- [kontoreiendom – knapp lovtekst + eksempel](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/avskrivninger_kontoreiendom_knapp_lovtekst_eksempel.md)
