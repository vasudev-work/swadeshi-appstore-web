# Swadeshi Appstore - web

The public web page for the Swadeshi Appstore catalogue: 1502 Made-in-India Android apps, searchable and grouped by category.

Live at https://vasudev-work.github.io/swadeshi-appstore-web/

## What it is

One self-contained `index.html`. No build step, no framework, no fonts or scripts loaded from a CDN. The app list is embedded in the page, so it works offline once loaded.

- Search across app name, developer and category
- Filter by category
- Light and dark theme, remembered on the device
- App icons load lazily from the app repository
- No ads, no analytics, no cookies, no account

## Editing the list

The list lives in the app repository as `app/src/main/assets/indian_apps.json`. The page embeds a trimmed copy of it (name, developer, category, link, icon id, package).

## Related repositories

- [swadeshi-store-android](https://github.com/vasudev-work/swadeshi-store-android) - the Android app
- [swadeshi-apps](https://github.com/vasudev-work/swadeshi-apps) - the list as a README
- [swadeshi-app-dictionary](https://github.com/vasudev-work/swadeshi-app-dictionary) - CSV and JSON data
- [awesome-indian-apps](https://github.com/vasudev-work/awesome-indian-apps) - apps plus open-source projects

## Licence

MIT. App names, icons and logos belong to their respective owners and are used only to identify the app.
