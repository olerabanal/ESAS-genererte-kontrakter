## Kvittering

Kvitterings-meldingen er tenkt brukt som en tilbakemelding på status for en gitt melding fra mottaker til avsender.

Hver kvitteringsmelding skal som minimum inkludere en egen _meldingsid_, en _referanseid_ til meldingen den svarer til, pluss en status på den refererte meldingen.

Dersom noe er feil på referansemeldingen skal kvitteringsmeldingen indikere om feilen ligger på avsenders eller mottakers side.
En kvitteringsmelding som indikerer feil bør også inneholde en beskrivelse om hva som har feilet.



### Noen prinsipper:

* Status **UNDER_MOTTAK** indikerer at meldingen er mottatt, men ikke ferdig prosessert inn i saksbehandlingssystem. Det kan fremdeles oppstå feil som gjør at avsender eller mottaker må starte feilsøking.
* Status **MOTTATT** indikerer at alt er ok. 
  * Avsender kan fjerne vedlegg fra filtjeneste når MOTTATT status er mottatt
  * Ingen nye kvitteringer forventes.
* Status **FEILET_AVSENDER** indikerer at det er noe feil hos avsender. F.eks. feil format, manglende vedlegg etc. Det er forventet av _avsender_ iverksette nødvendige tiltak for å sende melding på nytt.
  * En slik status skal aldri sendes etter at en MOTTATT melding er sendt
  * Ingen nye kvitteringer forventes.
* Status **FEILET_MOTTAKER** indikerer at det er noe feil hos mottaker. F.eks. bug eller system nede. Det er forventet at _mottaker_ undersøker.
  * en slik status skal aldri sendes etter at en MOTTATT melding er sendt
  * det forventes at det skal alltid komme en MOTTATT eller FEILET_AVSENDER kvittering i etterkant