# Peñagaricano Lab Website

**Quantitative Genomics & Computational Biology**  
Department of Animal & Dairy Sciences, University of Wisconsin-Madison

🌐 Website: [fpenagaricano-lab.org](https://fpenagaricano-lab.org)

---

## 🚀 Hosting on GitHub Pages

### Quick Setup
1. Create a new repository on GitHub (e.g., `penagaricano-lab.github.io` or `lab-website`)
2. Push all files to the `main` branch
3. Go to **Settings → Pages → Source → Deploy from a branch → main → / (root)**
4. Your site will be live at `https://yourusername.github.io/lab-website/`

### Custom Domain
To use `fpenagaricano-lab.org`:
1. In **Settings → Pages**, enter `fpenagaricano-lab.org` as the custom domain
2. Add these DNS records at your domain registrar:
   - `A` record pointing to `185.199.108.153`
   - `A` record pointing to `185.199.109.153`
   - `A` record pointing to `185.199.110.153`
   - `A` record pointing to `185.199.111.153`
   - `CNAME` record: `www` → `yourusername.github.io`

---

## Site Structure

```
├── index.html          # Home page
├── people.html         # Team members (current & alumni)
├── research.html       # Research areas
├── publications.html   # Publication list by year
├── software.html       # Software & tools (EnrichKit, greenfeedr)
├── news.html           # News & updates
├── opportunities.html  # Join us / open positions
├── style.css           # Global styles
├── images/             # Team photos & figures
│   └── (add photos here)
└── README.md           # This file
```

---

## ✏️ How to Update

### Adding a New Team Member
1. Open `people.html`
2. Copy an existing `person-card` div
3. Update the initials, name, role, and details
4. Commit and push

### Adding a New Publication
1. Open `publications.html`
2. Add a new `<li class="pub-item">` under the appropriate year
3. Bold `F Peñagaricano` in the author list
4. Link the title to the paper URL

### Adding News
1. Open `index.html`
2. Add a new `<div class="news-item">` in the news bar
3. Keep the most recent 4-5 items

### Adding Photos
1. Place photos in the `images/` folder
2. Replace `<div class="person-avatar">XX</div>` with:
   ```html
   <img src="images/firstname-lastname.jpg" alt="Name" class="person-avatar" style="font-size:0;">
   ```

---

## 🎨 Design System

- **Primary Color:** `#1a2744` (Navy)
- **Accent:** `#c9302c` (Wisconsin Red)  
- **Gold:** `#d4a843` (UW Gold)
- **Fonts:** Playfair Display (headings), Source Sans 3 (body), JetBrains Mono (code)

---

## TODO
- [ ] Add individual photos for all team members
- [ ] Add more publications (pre-2023) to publications.html
- [ ] Add Google Analytics tracking
- [ ] Add lab group photo to index.html

---

## 👥 Maintained By
- **Ümit Bilginer** (PhD Student) & **Francisco Peñagaricano** (PI)
- Department of Animal & Dairy Sciences, UW-Madison

*Last updated: February 2026*
