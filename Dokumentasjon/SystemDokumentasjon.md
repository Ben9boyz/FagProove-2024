<details open>
  <summary>
    <h2>Teknologier</h2>
  </summary>

  - #### Omega 365 NT (Appframe).
    
    - Innebygd sikkerhet: Omega 365 NT har innebygd sikkerhet.
    - Bedriftens standard : Omega 365 NT er en del av bedriftens standard.
    - Rikelig med komponenter: Omega 365 NT tilbyr en del komponenter.
        #### Teknologier innebygd i Appframe.
      - HighCharts: Brukt for å lage grafer
      - SQL Server: Brukt for datahåndtering og tilgangstyring
      - Vue.js: Brukt for FrontEnd utvikling
      - Bootsrap: For styling av FrontEnd

  - GitHub: Til dokumentering av prosjekte.
  - DrawSQL: Brukt for å lage SQL Tabell diagramm.
  - Figma: Brukt for skissing av apper

    
  <hr>
</details>
<details open>
  <summary>
    <h2>Arkitektur</h2>
  </summary>
<ul>
    <li>
      <details>
        <summary>
          <h4>Tabeller</h4>:
        </summary>      
        <a href="https://drawsql.app/teams/omega-1/diagrams/feedback-system-for-kundeservice-2/embed">Tabellstruktur</a>
          <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/3d32a234-53bc-4ef3-bb9c-5a8932c3222a" />
      </details>
    </li>
    <li>
      <details>
        <summary>
          <h4>Views</h4>: 
        </summary>
        <table>
          <tr>
            <th>View Navn</th>
            <th>Beskrivelse (Hvorfor eksisterer dette viewet?)</th>
            <th>Bilder</th>
          </tr>
          <tr>
            <td><b>aviw_BenjaminKOsnes_MyCapabilitiesOnCurrentOrgUnit</b></td>
            <td>
Dette viewet viser Capabilities du har i den contexten(OrgUnit_ID) du står i.
            </td>
            <td>
              <table>
                <th>
                  <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/78a73f71-caed-46f6-8b7e-399d8d816e8e" width="200" />
                </th>
              </table>
            </td>
          </tr>
          <tr>
            <td><b>aviw_BenjaminKOsnes_CompanyReviewsStatsAvgRatingOverTime</b></td>
            <td>
              Dette viewet henter ut va rating til bedriften var for hver gang det ble lagt in en anmeldelse
            </td>
            <td>
              <table>
                <th>
                  <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/99ffb8d2-bfd5-445b-bfba-6242c4d4badf" width="200" />
                </th>
              </table>
            </td>
          </tr>
          <tr>
            <td><b>aviw_BenjaminKOsnes_CompanyReviewsStats</b></td>
            <td>
                   Henter ut Statistikk om bedriftens anmeldeser
            </td>
            <td>
              <table>
                <th>
                  <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/76937ca7-ee89-4c3e-8439-97dc5a6451af" width="200" />
                </th>
              </table>
            </td>
          </tr>
          <tr>
            <td><b>aviw_BenjaminKOsnes_ReviewsCompanies</b></td>
            <td>
                   Henter ut alle bedrifter i systemet og anmeldelsene din på dem om det eksistere
            </td>
            <td>
              <table>
                <th>
                  <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/648063fe-3bd2-4b7e-926c-9dd9783afde4" width="200" />
                </th>
              </table>
            </td>
          </tr>
        </table>
      </details>
    </li>
    <li>
      <details>
        <summary>
          <h4>Stored Procedures</h4>:
        </summary>
        <table>
          <tr>
            <th>Stored Procedure Navn</th>
            <th>Beskrivelse</th>
            <th>Bilde</th>
          </tr>
          <tr>
            <td><b>astp_BenjaminKOsnes_CreateResponse</b></td>
            <td>
              Lager ny rad i response tabellen med Review_ID og Comment som blir sendt inn
            </td>
            <td>
              <table>
                <th>
                  <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/6bd74c1d-1d97-4e46-a9e2-5ec760b46c35" width="200" />
                </th>
              </table>
            </td>
          </tr>
                    <tr>
            <td><b>astp_BenjaminKOsnes_CreateReview</b></td>
            <td>
              Lager ny rad i Review tabellen med data om reviewen som parameter
            </td>
            <td>
              <table>
                <th> <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/08f87ced-2ae6-4b5e-b4f4-a0e09910e7a9" width="200" />
                </th>
              </table>
            </td>
          </tr>
                              <tr>
            <td><b>astp_BenjaminKOsnes_DeleteReview</b></td>
            <td>
              Sletter rad i Review tabellen bruker review_ID som paramter
            </td>
            <td>
              <table>
                <th> <img src="https://github.com/Ben9boyz/FagProove-2024/assets/167029110/cd373988-91c3-49e1-8533-bfbe3cd65bcb" width="200" />
                </th>
              </table>
            </td>
          </tr>
        </table>
      </details>
    </li>
  </ul>
  <hr />
</details>
<details open>
  <summary>
    <h2>Sikkerhet</h2>
  </summary>

### Autentisering og Tilgangsstyring i Appframe

Autentiseringen på nettsiden håndteres gjennom Appframe. Når brukerne besøker siden, møtes de først av en innloggingsside. Her får de valget mellom å logge inn med Microsoft-konto eller med SQL-innlogging ved å oppgi e-postadresse/telefonnummer og passord. Hvis brukeren velger Microsoft, skjer autentiseringen internt hos Microsoft, og det returneres en token som knyttes til brukeren i systemet.

I Appframe er tilgangsstyring satt opp gjennom tilgangstabeller. Brukere har roller, hvor rollen definerer hvilke moduler brukeren har tilgang til. Modulene inneholder data om hvilke apper brukeren kan få tilgang til og tabeller brukeren kan få data fra. Det står også om brukeren har tilgang til å redigere data (AllowEdit) og slette data (AllowDelete). Rollen de har kan også inneholde capabilities, spesifikke tilganger brukeren kan få. Hver rolle som tildeles må tildeles på en OrgUnit.

#### OrgUnit

OrgUnit-ene er bygget rundt en trestruktur der alle OrgUnit-ene vil ha én enkelt forelder. Disse OrgUnit-ene kan ha forskjellige typer, for eksempel Company, Department, Client, Project, osv. For å få tilgang til data må en bruker ha en rolle for en gitt OrgUnit.

Arv gir tilgang til OrgUnits under. Som standard arver brukere tilgang nedover i OrgUnit-strukturen, noe som betyr at hvis du har en rolle i en OrgUnit over, har du også samme rolle i alle OrgUnits under.

OrgUnits kan også ha "DoNotInherit" (arves ikke). For disse OrgUnit-ene er det ikke nok å ha en rolle i en OrgUnit lenger opp i hierarkiet. Bare brukere med en rolle direkte på den DoNotInherit-OrgUniten vil få tilgang.

#### Kontekst

Brukere har også OrgUnit-kontekst, dette definerer hvilke orgunit de har valgt å stå i. Brukeren vil bare se data på eller under OrgUnit de står i.

Eksempel:

![image](https://github.com/Ben9boyz/FagProove-2024/assets/167029110/2311de12-83f0-4e8c-bac8-ad86763db1ee)


#### Database Role
Vanlige Brukere får bare DataBase rollen af_user, denne gir brukeren bare tilgang til lese views, bruke procedure og å bruke funksjoner. De har ikke tilgang til å lese fra en tabell
  <hr />
  
### Info til Utvikler

Alle tabeller som blir opprettet i Appframe får en atbv(view med tilgangs sjekk).

Atbv'en inneholder som regel en whereclause som sjekker om du har role som gir deg tilgang til å se data i tabellen som atbv er basert på. Annen sikkerhet kan legges til også om nedvøndig
Utvikler kan opprette Aviw's når det skal skrives custom views disse viewsen må passe på å innholde en from for tilgangssjekk eller en atbv
Samme logikk som nevnt ovenfor gjelder for oppreting av stored procedurees eller functions

For logikk rundt sletting og redingering oppretes det Trigger på tabell: Insert Trigger, Update Trigger og Delete Trigger. I disse ligger det som regel en whereclause som sjekker om du har en role som gir deg tilgang til å slette eller redigere data
Utvikler kan også legge in egne sikkerhets sjekker eller egen logikk i disse trigggerne.

Logikk rundt OrgUnits må implementeres manuelt av utvikler

  Utviklere i system på passe på å bruke views som er atbv eller bruker atbv når de henter ut data. Ellers vil ikke dataen blir filtert på brukerens tilganger. Utikvler skal ikke lage aviws som ikke innholder noe from for sikkerhet
  
</details>
<details open>
  <summary>
    <h2>Tilgangs styring i FeedBack Systemet</h2>
  </summary>

## ReviewUser
Gir tilgang til Company Feedback appen, og lese, slette og redigeringstilgang i atbl_BenjaminKOsnes_CompanyReviews.
Kan ikke se andre brukeres reviews.

## ReviewStatisticsViewer 
Gir tilgang til Company Feedback stats appen, og lese og redigeringstilgang i atbl_BenjaminKOsnes_CompanyReviewsResponses.
Denne rollen gir brukeren Capabilitien CanViewCompanyReviews. Denne gir deg mulighet til å se andres reviews til companies som ligger på eller under OrgUnit de har fått rollen på. 
Dataene som vises til brukeren blir filtrert basert på hvilken kontekst de har i OrgUnit-treet.

## Triggere
Triggerene til tabellen tar seg hånd om at bruker ikke kan redigere eller slette andres reviews.
Har også sjekk på om bruker oppretter flere en en anmeldelse på samme bedrift

## Logikk i atbv
### atbv_BenjaminKOsnes_Reviews:

![image](https://github.com/Ben9boyz/FagProove-2024/assets/167029110/a9e6b832-d835-4849-82b9-53412c6dfc65)

### atbv_BenjaminKOsnes_ReviewsResponses:
![image](https://github.com/Ben9boyz/FagProove-2024/assets/167029110/92d6d218-6914-4c36-8a50-626b1010d6e7)

<hr />
</details>

# Grensesnittbeskrivelse

Feedback Systemet består av 2 apper:

## Company FeedBack
Appen har to visninger, en der du kan se dine anmeldelser og en for bedrifter du kan legge anmeldelser på. Brukeren oppretter en anmeldelse gjennom et skjema som inneholder Rating, E-post, Tittel, Kommentar, Dato og Telefonnummer. Brukerens navn blir hentet ut fra deres ID som blir lagret i CreatedBy_ID.

På siden med sine anmeldelser kan brukeren se svar fra bedrifter. De har også mulighet til å slette og redigere anmeldelsene sine.

## Company FeedBack Statistics
Her kan brukere som har fått ReviewStatisticsViewer-rollen se review statistikk på bedriften de står i og svare på anmeldelser. Det er sider en for generell statistikk og en for å se på anmeldelser.

### General
- #### Rating
  - Inneholder gjennomsnittlig vurdering og antall anmeldelser bedriften har fått. Har også prosentbokser under som viser fordeling av vurderinger.
- #### Graphs
  - Inneholder grafer om fordeling av vurderinger og kan bytte til en graf som viser vurderingenes utvikling over tid.
- #### Reviews
  - Viser hvor mange anmeldelser bedriften har svart på og hvor mange de ikke har svart på.
- #### UnansweredReviews
  - Viser tre anmeldelser bedriften ikke har svart på. Er skjult om det ikke er noen ubesvarte.

### Reviews
  - Viser en listevisning av anmeldelser, filtrert enten på ubesvarte anmeldelser eller besvarte anmeldelser. Mulighet til å svare ved bruk av tekstboks under anmeldelser på anmeldelser som ikke har svar.

<hr />

# Hindringer under utviklingen

- Hadde lyst på animasjon på TextArea ved utviding, fant ut at det ikke funket så bra nå man skal utvide TextArea boksen i etterkant.
- Fikk problemer pga at jeg satt opp appen min til å bruke libraries istedenfor moduler. Har ingen erfaring med library versjonen og dette er helt nytt i rammeverket. Funket ikke å gjøre getDataObjectById hele tiden så måtte sende dataObject ned via props.
- Hadde problemer med å generere grafer som ikke var synlige på, gjorde egt på onMounted event men siden graf boksene ikke var synlige feilet genereringen. Etter liten stund endte jeg opp å flytte grafene inn i egne components som hadde egen OnMounted event slik at de ikke ble generert når man bare åpnet siden, men heller når man byttet til taben de var på.
- Prøvde å bruke UNION ALL i en atbv istedenfor OR siden tenkte det ville gi bedre performance, dette funket ikke i praksis siden SQL ikke liker å gjøre insert på view med UNION ALL.

<hr />

# Avvik fra plan (Endringer under utvikling)

## TilgangsStying
Skulle egentlig bruke feltet representsCompany_ID i atbl_System_Persons for å finne ut hvilke bedrift du skulle se i statistikkappen. Fant ut mitt i utviklingen at bruker har tilgang å bytte til alle companies de har fått rolle med orgUnit mot company. Dette gjør at selv om du i utgangspunktet har bare fått rolle for å se data i f.eks. Omega Gourmet, kan du bytte represents til en annen bedrift. Dette skaper et sikkerhetshull. Derfor byttet jeg til OrgUnit struktur slik at bruker må spesifikt få rollen  på OrgUnit (Company) de skal kunne se statistikken til. Dette gjør det også enklere å dele ut tilgang siden bruker arver tilgang ned i treet. Det er også mye enklere å bytte mellom companies om du har tilgang, siden du kan bruke context selectoren oppe til venstre.
Fjernet Resposne_ID i Response tabellen, følte ikke det var nødvendig at bruker og bedrift kunne svare igjen på en response

## Mail Response
La til at bruker får mail med respons når bedrift svarer.

## Komponenter


  <h2>Kilder</h2>
  
  - [Bootstrap 5 Docs](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
  - [Vue.js Docs](https://vuejs.org/guide/introduction.html)
  - [ChatGPT](https://chat.openai.com/)
  - [Omega Docs](https://omega-nt.omega365.com/nt/docs?Area-ID=10004)
  - [Stack Overflow](https://stackoverflow.com/)
  - [High Charts](https://www.highcharts.com/docs/index)
  - [W3schools](https://www.w3schools.com/)
  - [Draw SQL](https://drawsql.app/)
  - [Figma](https://www.figma.com/)
  - [Dokumentasjon Template fra Arvid Wedtstein](https://github.com/ArvidWedtstein/Proove-Fagproove/blob/main/System_Documentation.md#detalje-side)
- **Ressurser**
  - Omega Kollegaer


 
<hr />
</details>
