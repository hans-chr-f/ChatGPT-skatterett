## Grensen mellom arbeidsinntekt og virksomhetsinntekt

### Modellparametre
- modell = gpt-4-0125-preview
- temperature = 0.5

### Kontekst
- skatteloven kap. 5 (hele)
- Skatte-ABC V-9-1 ril V-9-3

### Prompts
Vi tester flere ulike prompts. Ulike prompts gir ulike svar! For å legge inn lovtekst og tekst fra Skatte-ABC bruker vi koden {KONTEKST}. Når vi måter inn spørsmålene i modellen bytter vi ut {KONTEKST} med rettskildene. Merk at den første prompten nedenfor ikke har en slik {KONTEKST}. Da tester hva modellen klarer uten at den får norske rettskilder eksplisitt matet inn. 

- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt.
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST} Tenk trinn for trinn.
- Du er en norsk ekspert på skatterett som skal løse spørsmål om skatt. Vis alltid hvilket rettslig grunnlag du bygger på. Dersom du er i tvil, gjør nøye rede for hvorfor du er tvil. Legg vekt på å skrive et sammenhengende resonnement. Unngå å bruke punktlister. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse rettslige spørsmål om skatt. Bruk følgende metode. Formuler hva det rettslige spørsmålet dreier seg om. Finn det rettslige grunnlaget som regulerer spørsmålet. Finn alle argumenter som er relevante for spørsmålet. Vurder alle relevante argumenter og henvis til rettskilder der dette er relevant. Konkluder. Legg vekt på å skrive en sammenhengende tekst der du ikke bruker punktlister og nummereringer. Baser svaret på følgende kontekst: {KONTEKST}

### Tester
Vi har utviklet to sett av spørsmål: 
Vi tester også kvaliteten på svarene varierer med hvor mye kontekst (rettskilder) vi mater inn. XXXXX Her har vi brukt seks forskjellige alternativer: 1) ingen kontekst, 2) bare lovetekst, 3) lovtekst + Skatte-ABC, 4) lovtekst pluss et eksempel på hvordan avskrivninger skal regnes ut, 5) knappp lovtekst og 6) knapp lovtekst + eksempel.

#### Welshman
- [Welshman – uten kontekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/welshman_uten_kontekst.md)

#### Sjakk
