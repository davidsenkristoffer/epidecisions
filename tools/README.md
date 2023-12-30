# Verktøy for oppretting av ADR
- For å standardisere beslutningsfortegnelser i et prosjekt, anbefales det å bruke CLI-verktøyet `adr-tools`.
- For å komme i gang, følg oppstartsveiledningen her: https://github.com/npryce/adr-tools#quick-start

## TL:DR;

### Initialiser verktøyet for ditt prosjekt

- `adr init` i roten av ditt prosjekt.
  - Standardstien er `doc/architecture/decisions`, men den kan overstyres om ønskelig.

### Opprette et nytt dokument

- `adr new <navn på dokument>`

### Erstatte et eksisterende dokument

- Dersom du har et eksisterende beslutningsdokument som du ønsker å erstatte, kjør denne kommandoen:
- `adr new -s <nummer på gammelt dokument> <navn på dokument>`

### Hjelp

- `adr help`