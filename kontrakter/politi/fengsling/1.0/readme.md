## Versjon 1.0 som vi til slutt skal gå i produksjon med i ESAS II
Det er ikke laget eksempel på melding når kjennelsen kommer fra domstolene og den blir sendt videre til Kriminalomsorgen.
Detaljert lovreferanse (lovreferanseElement) er ikke en del av eksempelet og trenger justering. Type kan kanskje være en enum (utvidbar?) med PARAGRAF, LEDD....
Vi kommer til å implementere til slutt 
###### Samlet Json Schema for Kriminalomsorgen
Ny schema som ikke refererer til felles skjema for Kriminalomsorgen. 
* innsettelsesordre.combined.schema.json - er samme som innsettelsesordre.json
* oppdaterVaretekt.combined.schema.json - er samme som oppdaterVaretekt.schema.json
Sammenslåingen av schema er gjort manuelt i første omgang, skal lage en utility som fikser det automatisk slik at vi slipper å vedlikeholde 2 versjoner av schema.

Versjon 1.0 er synket med felles schema for [begjæring om varetekt](../../varetekt/reamde.md) samt at alle detaljer er med.
[Versjon 0.9](../0.9/readme.md)