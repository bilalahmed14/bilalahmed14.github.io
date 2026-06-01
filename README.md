# Bilal Ahmed — Software Solutions Site

Static single-page site. No build step, no dependencies.

## Form: How it works

The contact form uses [Web3Forms](https://web3forms.com) (FormSubmit.co has been
unreliable / down). Submissions are emailed to **bilalahmed3840@gmail.com**.

**One-time setup (about 30 seconds):**

1. Open [web3forms.com](https://web3forms.com) and enter `bilalahmed3840@gmail.com`.
2. Copy the **Access Key** from your inbox or the site.
3. In `index.html`, find `WEB3FORMS_ACCESS_KEY` and paste your key between the quotes.
4. Test the form on your **live site** or via `npx serve .` — opening `index.html` directly as a file will not work.

**Local testing:** Run `npx serve .` in this folder, then open `http://localhost:3000`.

## Deploy to Cloudflare Pages (free)

1. Push this folder to a GitHub or GitLab repo (or upload directly).
2. Go to [dash.cloudflare.com](https://dash.cloudflare.com) → **Workers & Pages** → **Create** → **Pages**.
3. Connect your Git repo, or choose **Direct Upload** and drag-drop this folder.
4. Set:
   - **Build command**: _(leave blank)_
   - **Build output directory**: _(leave blank, or `/` if required)_
5. Click **Deploy**. Your site will be live at `<project>.pages.dev` in under a minute.

## Deploy to Vercel (free)

1. Push this folder to a GitHub repo.
2. Go to [vercel.com/new](https://vercel.com/new), import the repo.
3. Framework preset: **Other**.
4. Leave build settings empty. Click **Deploy**.

## Files

- `index.html` — the full page (HTML + inline JS for form handling)
- `style.css` — all styles
- `README.md` — this file
