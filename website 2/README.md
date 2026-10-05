# Arianna's Cleaning Services — website

A simple, fast, one-page website: hero, about, services, and a contact
section with click-to-call, WhatsApp, email, and a map. No build step —
just plain HTML/CSS, so it works immediately on GitHub Pages.

## File structure

```
index.html
css/style.css
assets/logo.jpg        (logo mark used in the header and footer)
assets/hero-card.jpg   (the main card graphic shown in the hero section)
```

## Go live on GitHub Pages today

1. **Create a new repository** on GitHub (e.g. `ariannas-cleaning`). Keep it Public — GitHub Pages' free tier requires a public repo (unless you're on GitHub Enterprise/Pro with private Pages).

2. **Upload these files**, keeping the same folder structure:
   - Easiest way: on your new repo's page, click **Add file → Upload files**, then drag in `index.html`, the `css` folder, and the `assets` folder together.
   - Or, if you use git from a terminal:
     ```
     git init
     git add .
     git commit -m "Launch website"
     git branch -M main
     git remote add origin https://github.com/YOUR-USERNAME/ariannas-cleaning.git
     git push -u origin main
     ```

3. **Turn on Pages:**
   - In your repo, go to **Settings → Pages**.
   - Under "Build and deployment", set **Source** to **Deploy from a branch**.
   - Set **Branch** to `main` and folder to `/ (root)`, then **Save**.

4. **Wait about a minute**, then refresh that same Settings → Pages screen — GitHub will show your live URL, usually:
   ```
   https://YOUR-USERNAME.github.io/ariannas-cleaning/
   ```

That's it — no build tools, no npm install, nothing else to configure.

## Using your own domain (optional)

If you later buy a domain (e.g. `ariannascleaningservices.com`):
1. In **Settings → Pages**, enter it under "Custom domain."
2. At your domain registrar, add a CNAME record pointing to `YOUR-USERNAME.github.io`.
3. GitHub will auto-provision HTTPS for it after the DNS updates (can take a few hours).

## Editing content later

- **Phone/email/service area:** search `index.html` for `(805) 264-7008` and `arrianascleaningservicess@gmail.com` — each appears in a couple of places (header, hero, contact, footer).
- **Services:** edit the two `<ul>` lists inside the `id="services"` section.
- **Colors/fonts:** all in `css/style.css` at the top under `:root` — change the hex values there to re-theme the whole site at once.
- **Map:** the embedded map searches for "Santa Maria, CA." To point it at an exact address instead, replace the text after `q=` in the `src` of the `<iframe>` in the contact section.

## Notes

- The WhatsApp button links to `https://wa.me/18052647008` — this opens a chat with that number on WhatsApp from any device.
- The map embed and web fonts load from Google's servers, so an internet connection is needed to see them — normal for any live website, this just won't show in a fully offline preview.
