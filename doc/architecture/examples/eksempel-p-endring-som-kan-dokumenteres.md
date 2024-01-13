# 2. Miljøløftets skjemaløsning flyttes til Power Platform

Dato: 2023-06-30

## Status

Akseptert

## Kontekst

Miljøløftets skjemaløsning for innsending av søknader om pengestøtte har tradisjonelt vært en del av Episerver-løsningen. Denne var veldig kostbar å vedlikeholde, og utvikler måtte involveres på hver eneste endring.

## Beslutning

Miljøløftets skjemaløsning flyttes til Power Platform.

## Konsekvenser

Ny løsning er mye enklere for kunde å vedlikeholde, og behøver ingen (eller lite) involvering fra utviklere. Bouvet har egne spesialister på Power Platform som overtar ansvaret for løsningen. Det er blitt enklere å integrere nye brukere, da pålogging med Azure AD fungerer sømløst med Power Platform.
En ulempe med ny løsning er at Power Platform er veldig populært, og dermed øker sannsynligheten for angrep mot potensielle svakheter i applikasjonen. Et eksempel på dette var da det ble avdekket en svært alvorlig sårbarhet i Power Platform Connectors (CVSS score 9.6 / 10) i desember 2023.

## Relatert

Spoofing vulnerability i Power Platform Connectors: https://msrc.microsoft.com/update-guide/vulnerability/CVE-2023-36019