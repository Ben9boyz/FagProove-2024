### App 1: KundeApp for å legge inn og se egne reviews

 **Visning av Bedrifter:**
   - liste av Bedrifter som man kan gi anmeldelse på
   - Knapp for å lage ny anmeldelse og knapp for å se gamle anmeldelser

 **Innlegging av reviews:**
   - Brukere skal kunne fylle ut et skjema for å legge inn nye reviews.
   - Skjemaet bør inneholde felt for Kommentar, dato/tid for hendelse, tlfnummer, Email og stjernerangering(1-5). Om bruker ikke skriver tlf eller email, vil det de har koblet opp mot brukeren sin bli brukt
   - Ikke mulighet for å legge inn review på samme hendelse

 **Oversikt over gamle reviews:**
   - Brukere skal kunne se en liste over alle reviews de har lagt inn tidligere.
   - Hvert review i listen skal vise teksten i anmeldelsen og stjernerangeringen.
   - Mulighet til å redigere gamle reviews
     
 **Svarfunksjonalitet:**
   - Brukere skal kunne svare på responsen til egne reviews.
   - Svar bør kunne legges inn direkte under det tilsvarende reviewet.
     
 **TilgangsStyring**
   - For å ha tilgang til denne appen må man få rollen Review User, man skal kun kunne se Reviews man selv har lagt inn og besvarelse på den.
     
### App 2: BedriftsApp for å se og svare på reviews

 **Dashboard med oversikt:**
   - Et dashbord skal vise gjennomsnittlig rating for bedriften basert på alle reviews.
   - Diagrammer eller grafer kan brukes til å visualisere ratingfordelingen eller trendene over tid.

 **Liste over ubesvarte reviews:**
   - Bedriften skal ha tilgang til en liste over alle reviews som ikke har fått et svar enda.
   - Dette kan hjelpe bedriften med å sikre at ingen reviews blir oversett eller ignorert.

 **Svarfunksjonalitet:**
   - Bedriften skal kunne svare på reviews direkte fra appen.
   - Svar bør kunne legges inn under det tilsvarende reviewet for å skape en dialog med kunden.

 **Anmeldelsesvisning:**
   - Det skal være en enkel måte for bedriften å se alle reviews de har mottatt, inkludert tekst og rating.

 **TilgangsStyring**
   - For å ha tilgang til denne appen må man få rollen Review Viewer, du vil kun kunne se bedriften du står som representant til i Appframe(se datamodell)
