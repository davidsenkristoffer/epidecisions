# 2. Skyssloggen Azure B2C

Date: 2023-10-01

*Dersom det er nødvendig, sett inn beslutningstakere*

## Status

Akseptert

## Context

I dagens løsning av Skyssloggen benyttes det SQL-brukere til pålogging. 
For å få en sikrere og mer brukervennlig løsning ønsker vi å flytte pålogging til Azure AD.
Siden det kommer brukere fra flere forskjellige bedrifter / offentlige instanser, må vi kunne forene alle brukerkontoer i én påloggingsløsning.

## Decision

Skyssloggen tar i bruk pålogging med Azure AD og B2C til fordel for SQL-brukere.

## Consequences

Løsningen er tryggere fordi man kan lettere kan ta i bruk MFA som en del av påloggingsflyt. 
Man kan legge til rette for at brukere kan benytte pålogging med andre AD-kontoer samt Gmail- og Hotmailkontoer.
En negativ konsekvens med denne løsningen er at man behøver mer kompetanse innen Azure B2C, som ikke alle har. Det er også mer vedlikehold i form av rullering av nøkler i Azure, oppsett av påloggingsflyter og registreringsflyter m.m.

## Related

*Lenke til f.eks. Jira*
