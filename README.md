# northspirestudio.com

A minimal website for Northspire Studio, hosted free on GitHub Pages:

- `index.html`: home page
- `remotetv/privacy.html`: RemoteTV privacy policy (linked from the app's Settings and the Play listing)
- `app-ads.txt`: required by AdMob; put your publisher ID in it first
- `CNAME`: tells GitHub Pages to serve the site at northspirestudio.com

## Put it online

1. Create a free GitHub account, then a new **public** repository (any name, e.g. `website`).
2. Upload everything in this folder, keeping the `remotetv` subfolder.
3. Repository **Settings > Pages**: Source "Deploy from a branch", branch `main`, folder `/ (root)`, Save.
4. At the company where you bought northspirestudio.com, open the DNS settings and add:
   - four **A** records for `@` (the bare domain): `185.199.108.153`, `185.199.109.153`,
     `185.199.110.153`, `185.199.111.153`
   - one **CNAME** record for `www` pointing to `<your-github-username>.github.io`
   Leave the existing **MX** and **TXT** records alone: those keep Zoho Mail working.
5. Back in Settings > Pages, wait until the domain check passes (minutes to a few hours), then tick
   **Enforce HTTPS**.
6. Check https://northspirestudio.com/remotetv/privacy.html opens, then paste that address into
   Play Console's privacy policy field and put https://northspirestudio.com in the store listing's
   Website field (AdMob looks for app-ads.txt there).
