# Sanskar Travels 🌍

A personal travel blog — static HTML/CSS site, no build tools required.

## Files

- `index.html` — homepage with hero, destination cards, about section
- `sri-lanka.html` — 8-day Sri Lanka diary
- `oman.html` — 7-day Oman diary
- `thailand.html` — 7-day Thailand diary
- `vietnam.html` — 9-day Vietnam diary
- `georgia.html` — 9-day Georgia diary
- `styles.css` — shared styling (warm travel-journal theme)
- `images/` — custom destination illustrations (SVG, no external image hosting needed)

Just open `index.html` in a browser to preview locally — no installs needed.

To add a new country diary later: copy `sri-lanka.html`, swap the content, and add a new card to `index.html`'s destination grid.

## Free hosting — pick one

### Option A: GitHub Pages (recommended, free forever)

1. Create a free GitHub account at github.com if you don't have one.
2. Create a new repository (e.g. `wanderlust-diaries`), set it to **Public**.
3. Upload all files in this folder to the repo (drag-and-drop on the GitHub website works, or via git):
   ```
   cd /Users/sanskarsoni/Desktop/SanskarTravels
   git init
   git add .
   git commit -m "Initial travel blog"
   git branch -M main
   git remote add origin https://github.com/<your-username>/wanderlust-diaries.git
   git push -u origin main
   ```
4. In the repo, go to **Settings → Pages**.
5. Under "Source", select branch `main`, folder `/ (root)`, then **Save**.
6. Wait ~1 minute — your site will be live at:
   `https://<your-username>.github.io/wanderlust-diaries/`

### Option B: Netlify Drop (fastest, no account needed to start)

1. Go to **app.netlify.com/drop**.
2. Drag the whole `SanskarTravels` folder onto the page.
3. Netlify instantly gives you a live URL like `https://random-name.netlify.app`.
4. (Optional) Sign up free to keep the site permanently and get a custom subdomain like `wanderlust-diaries.netlify.app`.

### Option C: Vercel

1. Sign up free at vercel.com (can use GitHub login).
2. Click "Add New → Project", import your GitHub repo (from Option A), or drag-and-drop the folder.
3. Deploy — Vercel gives you a URL like `https://wanderlust-diaries.vercel.app`.

## Optional next steps

- **Custom domain**: Buy a domain (e.g. from Namecheap, ~$10/year) and point it at your GitHub Pages/Netlify/Vercel site — all three support free custom domain connection.
- **Real photos**: Replace the gradient placeholder blocks (`.dest-card .bg`, `.gallery-strip div`, `.about-photo`) with your own photos — add an `images/` folder and update the CSS `background-image` or swap in `<img>` tags.
- **Newsletter signup**: The email form on the homepage is currently a placeholder. To make it functional for free, connect it to [Formspree](https://formspree.io) (free tier) or [Mailchimp](https://mailchimp.com) — both just require replacing the form's `action` attribute with the URL they give you.
- **Analytics**: Add a free [Plausible](https://plausible.io) or [Google Analytics](https://analytics.google.com) snippet before `</head>` if you want visitor stats.
