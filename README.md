# fotballloggen-web

Den offentlige nettsiden for **FotballLoggen**. Appkoden ligger i et eget,
privat repo – dette repoet finnes fordi GitHub Pages ikke virker på private
repoer uten betalt plan, og fordi disse sidene *må* være offentlige:

| Side | Hvorfor den må være offentlig |
| --- | --- |
| `apne/index.html` | Landingssiden QR-kodene i appen peker på |
| `privacy.md` | Personvernerklæring – påkrevd URL i App Store Connect |
| `support.md` | Support-URL – påkrevd i App Store Connect |
| `index.md` | Forside / marketing-URL |

## Landingssiden (`/apne/`)

QR-kodene i appen inneholder ikke deeplinks, men en https-lenke hit:

```
/apne/?code=ABCD2345    → invitasjon til medforelder
/apne/?token=<32 hex>   → barn setter opp konto
```

Siden forsøker å åpne `fotballloggen://…`, og faller ellers tilbake til
nedlasting + invitasjonskoden i klartekst. Grunnen er at iOS-kameraet ikke
åpner ukjente URL-schemes fra QR, og at mottakeren ofte ikke har appen.

**Nedlastingslenken settes i `apne/index.html`:**

```js
var DOWNLOAD_URL = "https://testflight.apple.com/join/XXXXXXXX";
```

Så lenge den inneholder `XXXX` regnes den som ikke satt, og siden viser en
forklaring i stedet for en ødelagt lenke. Bytt til App Store-URL-en etter
lansering.

Test uten auto-åpning: legg på `&noauto=1`.

## Førstegangsoppsett

1. Opprett et **offentlig** repo `fotballloggen-web` på GitHub (uten README –
   dette repoet har allerede en).
2. Push:
   ```bash
   git remote add origin git@personal:ihneskarbovik/fotballloggen-web.git
   git push -u origin main
   ```
3. Settings → Pages → Deploy from a branch → `main` / `/ (root)` → Save.
4. Verifiser etter 1–2 minutter:
   - <https://ihneskarbovik.github.io/fotballloggen-web/>
   - <https://ihneskarbovik.github.io/fotballloggen-web/privacy>
   - <https://ihneskarbovik.github.io/fotballloggen-web/support>
   - <https://ihneskarbovik.github.io/fotballloggen-web/apne/?code=TEST1234>

Endrer du repo-navnet, må `WEB_BASE_URL` i appens `src/config/links.ts`
oppdateres og appen bygges på nytt. Selve siden kan endres når som helst
med en push – den er ikke en del av appbundelen.
