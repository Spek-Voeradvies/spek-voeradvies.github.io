# Spek Voeradvies — GitHub Pages website

Een responsive, Nederlandstalige bedrijfswebsite voor Spek Voeradvies, inclusief presentatie van Voerplanner. De website bestaat uit statische HTML, CSS en JavaScript en kan gratis worden gehost met GitHub Pages.

## Bestanden

- `index.html` — alle pagina-inhoud en secties
- `assets/styles.css` — vormgeving en responsive layout
- `assets/script.js` — mobiel navigatiemenu en automatisch jaartal
- `assets/favicon.svg` — browsericoon

## Eerst aanpassen

Open `index.html` en vervang in de contactsectie:
- `Vul hier je zakelijke e-mailadres in`
- `Optioneel: vul je telefoonnummer in`
- `JOUW-GEBRUIKERSNAAM.github.io`

Controleer ook alle beschrijvingen van diensten en Voerplanner. De Voerplanner-visual is nadrukkelijk een schematische illustratie, geen live screenshot.

## Publiceren via GitHub Pages

### Optie A — projectrepository (aanbevolen als je repository niet je gebruikerssite is)

1. Maak op GitHub een nieuwe **public** repository aan, bijvoorbeeld `spek-voeradvies-website`.
2. Upload de bestanden en mappen uit deze map naar de hoofdmap van de repository. `index.html` moet dus direct in de root staan.
3. Open in de repository **Settings → Pages**.
4. Bij **Build and deployment** kies je **Deploy from a branch**.
5. Kies branch `main` en map `/(root)`, klik **Save**.
6. Wacht op de deployment. De URL heeft deze vorm: `https://spek-voeradvies.github.io/Spek-Voeradvies/`.

### Optie B — gebruikerssite

Wil je de kortste URL zonder projectnaam, maak dan een repository die exact heet `JOUW-GITHUB-GEBRUIKERSNAAM.github.io`. Publiceer dezelfde bestanden vanaf `main` en `/(root)`. De URL wordt `https://JOUW-GITHUB-GEBRUIKERSNAAM.github.io/`.

## Controleren na publicatie

- Open de getoonde Pages-URL in een privévenster.
- Test de navigatie op desktop en mobiel.
- Klik alle menu-items en controleer contactgegevens.
- Controleer de site op een telefoon.
- Houd rekening met enkele minuten vertraging na een nieuwe deployment.

## Belangrijke aandachtspunten

- GitHub Pages host statische bestanden; deze website heeft geen backend nodig.
- Een contactformulier verstuurt op dit moment geen berichten. Gebruik voorlopig een zichtbaar e-mailadres of voeg later een formulierdienst/backend toe.
- Publiceer geen wachtwoorden, API-sleutels, Supabase `service_role`-sleutel of andere geheimen in deze repository.
- Google Fonts wordt extern geladen. Als je geen externe fontservice wilt gebruiken, verwijder dan de `@import` bovenaan `assets/styles.css`; de opgegeven fallback-lettertypen blijven beschikbaar.
- Gebruik voor de website een aparte repository. Dit houdt de publieke bedrijfswebsite gescheiden van de broncode en configuratie van Voerplanner.
