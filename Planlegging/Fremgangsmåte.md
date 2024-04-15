### Fremgangsmåte for å utvikle et Feedback-System for kundeService

#### Planleggingsfasen:

- **Funksjonalitet**
  Feed


- **Skissering av design og layout:**
  - Bruk Figma for å lage en skisse av design og layout til applikasjonen.
- **Oppretting av datamodell:**
  - Bruk SQL for å lage en skisse av datamodellen.

#### FrontEnd Utvikling:

- **Rammeverk og teknologier:**
  - Benytt Omega 365 New Tech rammeverket.
  - Bruk Vue.js, HTML, CSS, JavaScript og TypeScript for FrontEnd-utvikling.
- **Design med Bootstrap 5:**
  - Bootstrap 5 er innebygd i Appframe og er standarden.
  - Bruk Bootstrap for å skape et brukervennlig system med fokus på tilgjengelighet og enkel styling av applikasjonen.
  - Følg bedriftens rutine, minst mulig bruk av custom CSS der det lar seg gjøre.

#### Middle Layer:

- **Håndteres av Appframe(APIet):**
  - Sikkerhet mellom samspill med SQL server og frontend.

#### Backend Utvikling:

- **Bruk av Transact SQL Server:**
  - Håndter backend med Transact SQL Server.
  - Implementer Appframe sikkerhet og tilgangsstyring for å sikre dataen.
- **Data lagring:**
  - Lagre dataen på SQL Server.

#### Sikkerhet:

- **Tilgangskontroll:**
  - Bygg sikkerhet i SQL ved hjelp av Omegas innebygde tilgangsstyring.
  - Følg bedriftens standarder for tilgangskontroll.
  - Sikkerhet i SQL Views og SQL Triggere som er koblet opp mot Rammeverket tilgangstyings tabeller, i tråd med Omega standarder.
- **Innlogging:**
  - Lagring og håndtering av Brukernavn og passord er satt opp i Azure.
  - Login er koblet opp mot en login På Sql Server, login har oppkobling mot Database bruker i system.
  - Støtte for login via Microsoft, bruker kan ha begge innlogins typer.
