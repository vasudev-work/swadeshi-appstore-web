# Swadeshi Appstore - web

The public web page for the Swadeshi Appstore catalogue: 1502 Made-in-India Android apps, laid out like the Android app.

Live at https://vasudev-work.github.io/swadeshi-appstore-web/

## What it is

One self-contained `index.html`. No build step, no framework, nothing loaded from a CDN. The app list is embedded in the page, so it works offline once loaded.

## Layout

Same shape as the Android app:

- Top bar with the app name, a **Choose your OS** pill, and a theme switch
- Category chips: Top charts, Government, Fintech, Social, Games
- Two cards: **Check my phone** and **Know an Indian app we missed?**
- **Horizontal card carousel** per category, with a Swadeshi badge, Save, and Open / Govt / Website buttons
- **Suggested for you** list
- **Five-tab bottom bar**: Govt Apps, Apps, Search, Books, You
- **Choose your OS** sheet: All platforms, Android, macOS, Windows, Linux. Only Android has data, and the page says so instead of showing empty results

## What it does not do

- It cannot read the apps installed on your phone. That only works inside the Android app, and the page says so on the "Check my phone" card.
- It does not phone home. No ads, no analytics, no cookies, no account. Saved apps and theme live in `localStorage` on your device only.

## Editing the list

The list lives in the app repository as `app/src/main/assets/indian_apps.json`. This page embeds a trimmed copy of it (name, developer, category, subcategory, links, icon id, package).

## Related repositories

- [swadeshi-store-android](https://github.com/vasudev-work/swadeshi-store-android) - the Android app
- [swadeshi-apps](https://github.com/vasudev-work/swadeshi-apps) - the list as a README
- [swadeshi-app-dictionary](https://github.com/vasudev-work/swadeshi-app-dictionary) - CSV and JSON data
- [awesome-indian-apps](https://github.com/vasudev-work/awesome-indian-apps) - apps plus open-source projects

## Licence

MIT. App names, icons and logos belong to their respective owners and are used only to identify the app.
