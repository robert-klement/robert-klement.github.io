# Robert Klement — Personal Website

Academic personal website, structured similarly to [Daniel Huber's IFA page](https://home.ifa.hawaii.edu/users/dhuber/).

Live at: **https://robert-klement.github.io** (after setup below)

---

## Setup: GitHub Pages (one-time, ~5 minutes)

### 1. Create the repository

Go to [github.com/new](https://github.com/new) and create a new repository named exactly:

```
robert-klement.github.io
```

> **Important:** The repo name must be `<your-github-username>.github.io`.
> Leave it **Public** (required for free GitHub Pages).
> Do **not** initialize with a README.

### 2. Push this site to the repository

From your terminal, inside this folder:

```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/robert-klement/robert-klement.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to your new repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under *Build and deployment*, set **Source** to `Deploy from a branch`
4. Set **Branch** to `main`, folder to `/ (root)`
5. Click **Save**

Your site will be live at **https://robert-klement.github.io** within ~60 seconds.

---

## Updating the site

Edit `index.html` locally, then:

```bash
git add index.html
git commit -m "Update [what you changed]"
git push
```

GitHub Pages redeploys automatically on every push.

---

## What to fill in

Open `index.html` and search for `<!-- UPDATE` or `[brackets]` to find every placeholder:

| Placeholder | What to add |
|---|---|
| `[Position]` | e.g. *Postdoctoral Scholar* |
| `[Institution]` | e.g. *Caltech* |
| ORCID link | Your ORCID profile URL |
| Google Scholar link | Your Scholar profile URL |
| Email | your.name@institution.edu |
| Publications | Add entries following the existing pattern |
| Talks | Replace the placeholder blocks |
| Teaching | List courses you've taught / TA'd |
| Bio paragraph | 2–3 sentences about your background |

---

## Optional: custom domain

If you have a domain (e.g. `klement-astro.com`), you can point it to GitHub Pages:

1. In your DNS provider, add a CNAME record pointing to `robert-klement.github.io`
2. In GitHub repo → Settings → Pages, enter your custom domain

GitHub handles HTTPS automatically.
