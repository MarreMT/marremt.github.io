# marremt.github.io

Det här repot finns bara för att Android ska kunna verifiera att APK:n och webbplatsen hör ihop. Android letar efter filen på domänens rot, `https://marremt.github.io/.well-known/assetlinks.json`, och dit når inte repot `Veckohandla`, som ligger under `/Veckohandla/`.

- `.well-known/assetlinks.json` säger att appen `se.marremt.veckohandla` hör till webbplatsen. Ersätt den med filen från PWABuilder, eller klistra in fingeravtrycket där det står `ERSÄTT_MED_FINGERAVTRYCKET_FRÅN_PWABUILDER`.
- `.nojekyll` är tom och måste finnas. Annars döljer GitHub Pages mappar som börjar med punkt, och filen ovan blir osynlig.
- `index.html` skickar den som går till `https://marremt.github.io/` vidare till appen.

Kontrollera att `https://marremt.github.io/.well-known/assetlinks.json` visar filen i webbläsaren. Visar den 404 är `.nojekyll` eller publiceringen inte rätt inställd.
