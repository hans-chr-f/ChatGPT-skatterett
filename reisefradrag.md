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


#### Reisefradrag
- [reisefradrag – uten kontekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/reisefradrag_uten_kontekst.md)
- [reisefradrag – lov og forskrifter](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/reisefradrag_lov_forskrift.md)
- [reisefradrag – lov og forskrifter + skatte-abc](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/reisefradrag_lov_forskrift_abc.md)
