# The FSS Review — website

This folder is the complete first-draft website. It is a plain website with no build step: one page (`index.html`) and an `images` folder. Nothing needs installing.

```
fss-review-site/
├── index.html      ← the whole page: text, layout and styling
├── images/         ← the seven photographs the page uses
└── README.md       ← this guide
```

---

## Part 1 — Put it on GitHub (no command line needed)

1. **Unzip** `FSS-Review-site.zip` on your computer. You'll get a folder called `fss-review-site`.
2. Go to **github.com** and sign in.
3. Click the **+** in the top-right corner → **New repository**.
4. Fill in:
   - **Repository name:** `fss-review` (any name works)
   - **Public** or **Private** — either works with Vercel
   - Leave every other box unticked.
5. Click **Create repository**.
6. On the next page, find the line *"…or upload an existing file"* and click **uploading an existing file**.
7. Open the `fss-review-site` folder on your computer, select **everything inside it** (`index.html`, the `images` folder and `README.md`) and drag it onto the GitHub page.
   - Drag the *contents* of the folder, not the folder itself, so `index.html` ends up at the top level of the repository.
8. Wait for all the files to finish uploading, then click the green **Commit changes** button.

Your code is now on GitHub.

---

## Part 2 — Publish it with Vercel

1. Go to **vercel.com** and choose **Continue with GitHub** to sign in.
2. Click **Add New…** → **Project**.
3. Find `fss-review` in the list and click **Import**.
   - If it isn't listed, click **Adjust GitHub App Permissions** and give Vercel access to that repository.
4. On the configuration screen:
   - **Framework Preset:** `Other`
   - Leave **Build Command** and **Output Directory** empty.
5. Click **Deploy**.

After about a minute Vercel gives you a live address like `fss-review.vercel.app`. That's the site.

---

## Part 3 — Use your own domain (optional)

1. In Vercel, open the project → **Settings** → **Domains**.
2. Type your domain (for example `fssreview.org`) and click **Add**.
3. Vercel shows one or two DNS records. Log in wherever you bought the domain and add exactly those records.
4. The domain usually starts working within an hour.

---

## Making changes later

Every change you save on GitHub is published by Vercel automatically within a minute or two.

**To change some text:**
1. On GitHub, open the repository and click `index.html`.
2. Click the **pencil icon** (Edit this file).
3. Press **Ctrl+F** (or **Cmd+F** on a Mac) and search for the words you want to change.
4. Change only the words between the tags — leave anything inside `< >` alone.
5. Click **Commit changes…**, then **Commit changes** again.

**To replace a photo:** upload a new image into the `images` folder with exactly the same file name as the one you're replacing (GitHub → open `images` → **Add file** → **Upload files**). Keeping the same name means you don't need to touch `index.html`.

**For bigger changes:** edit the Word document of the copy, or describe the change to Claude, and ask for a new `index.html`. Then replace the old file on GitHub: open the repository → **Add file** → **Upload files** → drag in the new `index.html` → **Commit changes**. It overwrites the old one.

---

## Not working yet (on purpose)

These are placeholders until the services exist:

- **Subscribe form** — the button doesn't send anything yet. It needs connecting to a newsletter service (Kit, Substack, Buttondown, etc.).
- **Back the Review (£5 / £10 / £25)** — need links to a payment page (Stripe, Kit, Patreon, etc.).
- **Essay titles, "Pitching guidelines", footer links** — point to `#` until those pages exist.
- **Lead essay image** — still a marked box waiting for a Kūṭiyāṭṭam or Nāṭyaśāstra image.
- **Square-bracket placeholders** like `[Season 2027]`, `[£X per essay]`, `[5%]`, `[EMAIL]`, `[YEAR]`.

Before launch, confirm the rights for every photograph in `images/`.
