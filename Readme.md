# Expense Tracker

A monthly expense tracker with month, year and all-years views. Income is optional for every month,
so months without income are fine. Includes charts, budget progress, category tables, CSV export,
and automatic saving to a GitHub repository so any device shows the same entries.

## Publish it (GitHub Pages)
1. Upload `index.html` and this `README.md` to the main branch of this repository.
2. Open **Settings > Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
3. After a minute or two the app is live at `https://<your-username>.github.io/expense-tracker/`.

## Save your entries to GitHub
Entries are saved to a file called `expenses.json` in a separate **private** repository, so your numbers are never
public. This repository only holds the app.

1. Create a private repository for the data, for example `car-tracker-data`, with "Add a README file" ticked.
2. In the app open **Settings > Save to GitHub**. Your username and `car-tracker-data` are filled in.
3. Press **Create it on GitHub**. GitHub opens with the token name and the Contents permission filled in.
   Choose **Only select repositories**, pick your data repository, generate the token and copy it.
4. Paste the token into the app and press **Connect and sync**.
5. On another device press **Copy setup link for another device** here, send it to yourself and open it there.

If you already use the car tracker on a device, this app reuses its GitHub connection automatically, because both
pages are on the same `github.io` address. The data stays in its own file, so the two never mix.

## Good to know
- The token is kept in that browser only and never written to any repository. A setup link contains the token, so
  treat it like a password.
- If two devices save at the same moment, both sets of new entries are kept.
- Without a connection the app saves in the browser only. **Settings > Back up and export** downloads a backup file
  or a CSV for Google Sheets and Excel.

## If something does not work
- **The page shows "404" after you enable Pages:** wait a few minutes, and check the repository is public and the page
  address uses the repository name exactly (a name typed with a space becomes `expense-tracker` with a hyphen).
- **You still see an old version:** reload with Ctrl+Shift+R, or pull down to refresh on a phone.
- **"Could not reach GitHub":** the message in **Settings > Save to GitHub** names the reason. Try another network, and turn
  off any ad blocker or VPN that blocks `api.github.com`.
- **Anything else:** open **Settings > About and troubleshooting**. It shows the last problem the app hit.
