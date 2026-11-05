# Suurpedot – Peto design system

Staattinen, yhden tiedoston sivu (`index.html`). Kaikki kuvat, fontit ja skriptit on upotettu tiedostoon, joten erillisiä kansioita ei tarvita.

**Salasana:** `Peto26!`

> ⚠️ Salasanasuojaus on vain kevyt "verho". Se tarkistetaan selaimessa, ja salasana näkyy sivun lähdekoodissa. Jos repo on julkinen, kuka tahansa voi lukea sen. Älä laita sivulle mitään oikeasti luottamuksellista.

---

## Julkaisu GitHub Pagesiin (selaimella, ilman komentoriviä)

1. **Luo repo:** github.com → **+** (oikea yläkulma) → **New repository**.
   - Nimi esim. `peto-design-system`
   - Valitse **Public** (ilmaisella tilillä Pages toimii vain julkisissa repoissa)
   - Paina **Create repository**.
2. **Lataa tiedostot:** uuden repon sivulla klikkaa linkkiä **uploading an existing file**.
   - Pura zip ja raahaa sen sisältämät tiedostot (`index.html`, `README.md`, `.nojekyll`) ikkunaan.
   - Jos `.nojekyll` ei näy (piilotiedosto), sen voi jättää pois – sivu toimii ilmankin.
   - Paina **Commit changes**.
3. **Laita Pages päälle:** repossa **Settings** → vasemmalta **Pages**.
   - *Source:* **Deploy from a branch**
   - *Branch:* **main**, kansio **/ (root)** → **Save**.
4. **Odota 1–2 minuuttia** ja päivitä Pages-sivu. Ylös ilmestyy osoite muotoa
   `https://<käyttäjänimi>.github.io/peto-design-system/`
5. Avaa osoite ja syötä salasana.

## Päivittäminen myöhemmin

Repossa: **Add file** → **Upload files** → raahaa uusi `index.html` (korvaa vanhan) → **Commit changes**. Pages päivittyy minuutin parin sisällä.

## Komentoriviltä (vaihtoehto)

```bash
cd peto-design-system
git init && git add . && git commit -m "Peto design system"
git branch -M main
git remote add origin https://github.com/<käyttäjänimi>/peto-design-system.git
git push -u origin main
```

Sen jälkeen kohta 3 yllä (Settings → Pages).

## Huomioita

- Sivu tarvitsee JavaScriptin. Se toimii kaikissa moderneissa selaimissa.
- Tiedosto on n. 1,4 Mt – hyvin GitHubin rajojen sisällä.
- Jos haluat oikean suojauksen, vaihtoehtoja ovat esim. yksityinen repo + maksullinen GitHub-tili, Netlify/Vercel salasanasuojauksella tai Cloudflare Access.
