# Rekvirering av personundersøkelse
Versjon 1.0 er første versjon som vi skal i produksjon med.
* [JSON Schema](1.0/rekvirerePersonundersoekelse.schema.json)
* [Eksempler](1.0/eksempelfiler/)

[Se changelog for endringer](changelog.md)


## Avklaringer
### Utestående avklaringer
 Kontaktpersonen må oppgis for videre dialog.
 Er påtalejurist alltid kontaktpersonen i politiet? (Alt. separat, påkrevd felt - eller gjør jurist påbudt)


### Avklarte avklaringer
Den siktede må identifiseres sikkert (fnr/D-nr)  og ha bosted eller oppholdsadresse angitt.
Kriminalomsorgen bruker oppholdsadresse og bostedsadresse til å rute rekvireringen til rett ansvarlig friomsorgskontor.

Sikker identitet er nødvendig for å hente korrekte og sensitive personopplysninger fra kildene.

Evt. verger bør identifiseres med fødselsnummer for informasjonssikkerheten. (Dette gir en robusthet i tilfelle adressebytter, flere personer med like/liknende navn, etc.)

Merk at man kan rekvirere en PUM selv om siktede ikke er mindreårig per i dag. Det er alderen på gjerningstidspunktet som avgjør.

Formålet med undersøkelse, vurdering av hensiktsmessighet av fengsling etc. kan være utstrukturert i PDF i denne omgang.

KOG-delen kan også tas som fritekst - konfliktrådet ville potensielt ha nytte av en strukturering av dette, men de får ikke denne meldingen direkte i denne omgang. Potensielt forbedring i senere versjon.


## Ønsker / mangler
Synk adressemodell og adressetyper mot folkeregisterets modell her - og generelt?

Tolkespråk er ønsket. Det finnes p.t. støtte for "statsborgerskap" som dekker deler av behovet - men klarer vi noe mer her, er det ønskelig.

