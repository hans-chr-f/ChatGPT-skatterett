## Grensen mellom arbeidsinntekt og virksomhetsinntekt

### Modellparametre
- modell = gpt-4-0125-preview
- temperature = 0.5

### Kontekst
- skatteloven kap. 5 (hele)
- Skatte-ABC V-9-1 til V-9-3

### Dommer
- Rt-1985-644 (EMI)
- HR-2015-1133-A (Solér)
- HR-2017-628-A (Thingaard)
- HR-2017-627-A  (Raise)

Vi har fjernet partenes anførsler og tingretten og lagmannsrettens domsbegrunnelser der de er inntatt etter Høyesteretts domskonklusjon.


### Prompts
Vi tester flere ulike prompts. Ulike prompts gir ulike svar! For å legge inn lovtekst og tekst fra Skatte-ABC bruker vi koden {KONTEKST}. Når vi måter inn spørsmålene i modellen bytter vi ut {KONTEKST} med rettskildene. Merk at den første prompten nedenfor ikke har en slik {KONTEKST}. Da tester hva modellen klarer uten at den får norske rettskilder eksplisitt matet inn. 

- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt.
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse spørsmål om skatt. Baser svaret på følgende kontekst: {KONTEKST} Tenk trinn for trinn.
- Du er en norsk ekspert på skatterett som skal løse spørsmål om skatt. Vis alltid hvilket rettslig grunnlag du bygger på. Dersom du er i tvil, gjør nøye rede for hvorfor du er tvil. Legg vekt på å skrive et sammenhengende resonnement. Unngå å bruke punktlister. Baser svaret på følgende kontekst: {KONTEKST}
- Du er en ekspert på norsk skatterett som skal løse rettslige spørsmål om skatt. Bruk følgende metode. Formuler hva det rettslige spørsmålet dreier seg om. Finn det rettslige grunnlaget som regulerer spørsmålet. Finn alle argumenter som er relevante for spørsmålet. Vurder alle relevante argumenter og henvis til rettskilder der dette er relevant. Konkluder. Legg vekt på å skrive en sammenhengende tekst der du ikke bruker punktlister og nummereringer. Baser svaret på følgende kontekst: {KONTEKST}

### Tester
Vi har utviklet to sett av spørsmål: Ett sett der spørsmålet er om en musikers inntekt er arbeidsinntekt eller virksomhetsinntekt (Welshman) og ett sett der spørsmålet er om aktivitet knyttet til en sjakkklubb er arbeidsinntekst eller virksomhetsinntekt (sjakk).
Vi tester også om kvaliteten på svarene varierer med hvor mye kontekst (rettskilder) vi mater inn. Her har vi brukt fire forskjellige alternativer: 1) ingen kontekst, 2) bare lovetekst, 3) lovtekst + Skatte-ABC, 4) lovtekst pluss en utdrag fra en dom (EMI-dommen) som behandler samme type spørsmål.

#### Welshman
- [Welshman – uten kontekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/welshman_uten_kontekst.md)
- [Welshman – bare lovtekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/welshman_bare_lovtekst.md)
- [Welshman – med lovtekst + skatte-abc](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/welshman_lovtekst_abc.md)

#### Sjakk
- [Sjakk – uten kontekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/sjakk_uten_kontekst.md)
- [Sjakk - bare lovtekst](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/sjakk_bare_lovtekst.md)
- [Sjakk – med lovtekst + skatte-abc](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/sjakk_lovtekst_abc.md)
- [Sjakk – lov og 4 dommer](https://github.com/hans-chr-f/ChatGPT-skatterett/blob/main/sjakk_lov_dommer.md)
