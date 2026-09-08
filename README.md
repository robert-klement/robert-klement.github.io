# Robert Klement — Personal Website

Academic personal website. Live at **https://robert-klement.github.io** after setup.

---

## One-time GitHub Pages setup (~5 min)

### 1. Create the repository

Go to [github.com/new](https://github.com/new) and create a repo named exactly:
```
robert-klement.github.io
```
Set it to **Public**. Do not initialize with a README.

### 2. Push this folder

From your terminal, inside this folder:
```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/robert-klement/robert-klement.github.io.git
git push -u origin main
```

GitHub Pages deploys automatically from the `main` branch. The site goes live within ~60 seconds.

### Every update after that:
```bash
git add .
git commit -m "describe what changed"
git push
```

---

## Files in this repo

| File | Purpose |
|---|---|
| `index.html` | The entire website (single file) |
| `Robert_Klement_CV.pdf` | Linked from the "Download CV" button |
| `photo.jpg` | **Add this yourself** — your profile photo |
| `README.md` | This file |

---

## Adding your photo

1. Add a photo of yourself to this folder, named **`photo.jpg`**
2. Recommended: square crop, at least 200×200 px
3. `git add photo.jpg && git commit -m "Add photo" && git push`

The site shows your initials "RK" as a fallback if `photo.jpg` is missing.

---

## Keeping content up to date

Open `index.html` and search for sections you want to update:

- **Publications** — add entries following the existing `<li>` pattern; update the stat numbers in `.pub-stats` when your citation count changes
- **Talks** — duplicate a `.ruled-item` block and fill in the details
- **Teaching / Service** — same pattern
- **CV** — replace `Robert_Klement_CV.pdf` with your updated file; keep the same filename, or update the `href` in the sidebar

---

## Optional: custom domain

If you have a domain (e.g. `klement-astro.com`):
1. Add a CNAME record in your DNS pointing to `robert-klement.github.io`
2. In GitHub repo → Settings → Pages → enter your custom domain
3. GitHub handles HTTPS automatically
