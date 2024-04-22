<details open>
  <summary>
    <h2>Teknologier</h2>
  </summary>

  - #### Omega 365 NT (Appframe).
    
    - Innebygd sikkerhet: Omega 365 NT har innebygd sikkerhet.
    - Bedriftens standard : Omega 365 NT er en del av bedriftens standardverktøy.
    - Rikelig med komponenter: Omega 365 NT tilbyr et bredt spekter av komponenter.
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

  <hr />
</details>
<details open>
  <summary>
    <h2>Grensesnittbeskrivelse</h2>
  </summary>
 
  <hr />
</details>

<details open>
  <summary>
    <h2>Hindringer under utviklingen</h2>
  </summary>

  <hr />
</details>

<details open>
  <summary>
    <h2>Avvik fra plan</h2> (Endringer under utvikling)
  </summary>
  

  <hr />
</details>
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
  - [Dokumentasjon Template fra Arvid Wedtstein](https://github.com/ArvidWedtstein/Fagproove/tree/main)
- **Ressurser**
  - Omega Kollegaer


 
<hr />
</details>
