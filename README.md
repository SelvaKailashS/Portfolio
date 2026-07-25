# Selva Kailash S — Portfolio

A classical-antiquity themed portfolio website — stone, parchment, gold leaf, and laurel motifs — built for a Computer Science & Engineering student who works across software and embedded hardware.

**Live demo:** _add your Vercel URL here after deploying_

![Theme](https://img.shields.io/badge/theme-ancient%20%2F%20classical-c9a227) ![Stack](https://img.shields.io/badge/stack-HTML%20%2F%20CSS%20%2F%20JS-2b2420)

---

## ✦ Features

- **Hero** — rotating armillary sphere emblem, animated laurel dividers, floating gold dust
- **Tablets of Knowledge** — carved-stone skill cards
- **The Chronicles** — parchment-style project cards with torn edges, wax-seal icons, and links to each project's GitHub repo (or a fallback source)
- **The Academy** — education and certifications, styled as pillar cards and tomes
- **The Gate** — contact section with a "Leave a Word" form that opens the visitor's email client, pre-addressed and pre-filled, so messages land straight in your inbox
- **Ancient mathematics watermark** — faint background diagrams (Pythagorean theorem, golden ratio, π, Euler's identity, Fibonacci sequence) woven throughout the page
- Scroll-triggered "unfurl" animations, a 3D tilt effect on project cards, and full mobile responsiveness

---

## ✦ Tech Stack

- Plain **HTML5** and **CSS3** (no build step, no framework)
- Vanilla **JavaScript** for scroll reveals, the tilt effect, and the contact form
- [Google Fonts](https://fonts.google.com/) — `Cinzel`, `Cinzel Decorative`, `Cormorant Garamond`
- [Font Awesome](https://fontawesome.com/) — icon set (loaded via CDN)

---

## ✦ File Structure

```
.
├── index.html      # all page content and structure
├── style.css        # all styling, layout, and animation
└── README.md
```

---

## ✦ Running Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   cd <your-repo>
   ```
2. Open `index.html` directly in a browser, **or** use the VS Code "Live Server" extension for auto-reload:
   - Right-click `index.html` → **Open with Live Server**

No build tools, package installs, or servers required — it's a static site.

---

## ✦ Deploying to Vercel

### Option A — Import from GitHub (recommended)

1. Push this project to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub.
3. Click **Add New → Project**, then select your repository.
4. Vercel will detect it as a static site automatically:
   - **Framework Preset:** Other
   - **Build Command:** _(leave blank)_
   - **Output Directory:** _(leave blank, or `.`)_
5. Click **Deploy**. Vercel will give you a live URL (e.g. `your-repo.vercel.app`) within seconds.

Every future push to `main` will auto-redeploy.

### Option B — Deploy via Vercel CLI

```bash
npm install -g vercel
cd <your-repo>
vercel
```

Follow the prompts (link to your Vercel account, confirm project settings), and it will deploy immediately. Run `vercel --prod` to push to your production URL.

---

## ✦ Customizing

- **Contact details** — update the email, phone, GitHub, and LinkedIn links in the `hero-meta` and `.gate-links` sections of `index.html`.
- **Projects** — each project lives inside a `<article class="scroll-card">` block in the "Chronicles" section; duplicate a block to add a new one.
- **Colors** — all theme colors are CSS variables at the top of `style.css` under `:root` (e.g. `--gold`, `--parchment`, `--bronze`) — change them there to re-theme the whole site.
- **Contact form** — the "Leave a Word" form currently opens a `mailto:` link addressed to `selvakailash95@gmail.com`. To change the recipient, edit the address inside the `messageForm` submit handler near the bottom of `index.html`.

---

## ✦ License

Personal portfolio — feel free to fork for inspiration, but please don't republish the content as your own.

---

Built by **Selva Kailash S** · Tirunelveli, India
