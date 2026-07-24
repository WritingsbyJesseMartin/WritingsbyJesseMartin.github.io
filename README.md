# Writings by Jesse Martin — setup instructions

## 1. Create the GitHub repo
1. Go to github.com, click **New repository**.
2. Name it `yourusername.github.io` (replace `yourusername` with your actual GitHub username — this exact naming is what makes GitHub Pages serve it automatically).
3. Set it to **Public**. Don't add a README/gitignore/license — leave it empty.

## 2. Upload these files
1. On the new repo's page, click **Add file → Upload files**.
2. Drag in everything from this folder (keep the folder structure — `_layouts`, `_posts`, `assets`, `_config.yml`, `index.html`).
3. Commit the changes.

## 3. Turn on GitHub Pages
1. In the repo, go to **Settings → Pages**.
2. Under "Build and deployment," set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Save. Wait 1–2 minutes. Your site will be live at `https://yourusername.github.io`.

## 4. Add a custom domain (optional, ~$10/year)
1. Buy a domain (Cloudflare Registrar, Namecheap, or Porkbun).
2. In your DNS settings, add a CNAME record pointing to `yourusername.github.io`.
3. Back in repo Settings → Pages, enter your custom domain in the "Custom domain" field.

## 5. Publish a new post
1. Go to the `_posts` folder on GitHub, click **Add file → Create new file**.
2. Name it `YYYY-MM-DD-your-title.md` (today's date, then a short slug — e.g. `2026-07-24-on-the-funding-formula.md`).
3. Paste this at the very top, then your text below it:
   ```
   ---
   layout: post
   title: "Your Post Title"
   ---

   Your writing starts here. Use ## for a header if you want one.
   ```
4. Click **Commit changes**. Live in about a minute.

That's the whole workflow — no coding needed after initial setup.
