### Fremgangsmåte for å utvikle et Feedback-System for KundeService

#### Planleggingsfasen:

- **Skissering av design og layout:**
  - Bruk Figma for å lage en skisse av design og layout til applikasjonen.
- **Oppretting av datamodell:**
  - Bruk Draw SQL for å lage en skisse av datamodellen.

#### FrontEnd Utvikling:

- **Rammeverk og teknologier:**
  - Benytter Omega 365 New Tech rammeverket(Appframe).
  - Appframe benytter Vue.js, HTML, CSS, JavaScript og TypeScript for FrontEnd-utvikling.
  - Bruke HighCharts til å lage Diagramer i dashbordet
- **Design med Bootstrap 5:**
  - Bootstrap 5 er innebygd i Appframe og er standarden.
  - Bruk Bootstrap for å skape et brukervennlig system med fokus på tilgjengelighet.
  - Følg bedriftens rutine, minst mulig bruk av custom CSS der det lar seg gjøre.
  - Ivareta Universel Utforming ved hjelp av Bootstrap.

#### Middle Layer:

- **Håndteres av Appframe(APIet):**
  - Sikkerhet og samspill mellom SQL server og frontend håndteres av Rammeverket

#### Backend Utvikling:

- **Data lagring:**
  - I Omega Benytter vi Transact SQL Server for lagring av dataer
- **DataModell:**
  - Bruke mest mulig innebygde tabeller i rammeverket til datamodell   

#### Sikkerhet:

- **Tilgangskontroll:**
  - Bygg sikkerhet i SQL ved hjelp av Omegas innebygde tilgangsstyring.
  - Følg bedriftens standarder for tilgangskontroll.
  - Sikkerheten i SQL Views og SQL Triggere som er koblet opp mot Rammeverket tilgangstyings tabeller, i tråd med Omega standarder.
