# Getting Verdict Ledger onto your iPhone home screen

You have 5 files: `index.html`, `manifest.json`, `icon-180.png`, `icon-192.png`, `icon-512.png`, `favicon-32.png`. They need to live on a real website address (not just in this chat) so the app can call out to the internet. GitHub Pages gives you that for free, with no coding tools required.

## 1. Create a free GitHub account (skip if you have one)
Go to [github.com/join](https://github.com/join) and sign up.

## 2. Create a new repository
- Click the **+** in the top right → **New repository**.
- Name it something like `verdict-ledger`.
- Set it to **Public**.
- Click **Create repository**.

## 3. Upload the files
- On the new repo's page, click **uploading an existing file** (or **Add file → Upload files**).
- Drag in all 6 files listed above.
- Scroll down and click **Commit changes**.

## 4. Turn on GitHub Pages
- Go to the repo's **Settings** tab → **Pages** (left sidebar).
- Under "Build and deployment," set **Source** to **Deploy from a branch**.
- Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
- Wait about a minute, then refresh — GitHub will show you a URL like:
  `https://YOUR-USERNAME.github.io/verdict-ledger/`

## 5. Add it to your iPhone home screen
- Open that URL in **Safari** on your iPhone (must be Safari, not Chrome).
- Tap the **Share** icon (square with an arrow) → **Add to Home Screen** → **Add**.
- A "Verdict Ledger" icon appears on your home screen and opens full-screen, like an app.

## 6. Add your Anthropic API key
- Open the app, tap the gear icon (⚙︎) top right.
- Get a key at [console.anthropic.com](https://console.anthropic.com/settings/keys) (sign up if needed, add a small amount of credit under **Billing**).
- Paste the key in, pick a model, tap **Save**.
- Optional but smart: in the Anthropic console under **Billing → Usage limits**, set a monthly spend cap (e.g. $5) as a safety net, since the key lives in your browser.

That's it — type or voice-type a claim and tap **Check claim**. Each check costs roughly a cent or two.

### Notes
- Your API key is stored only in Safari's local storage on your phone — it's sent straight from your phone to Anthropic's servers, nowhere else.
- Your ledger (past checks) is also stored locally on your phone. Use the **Export ledger** button in Settings occasionally to back it up as a JSON file, since clearing Safari's website data would erase it.
- To update the app later, just re-upload a changed `index.html` to the same GitHub repo — your home screen icon will pick up the change next time you open it.
