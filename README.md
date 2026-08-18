# Folio releases

Install packages for **Folio** — a portfolio site for visual artists: a Gallery of artwork and a Journal of the writing behind it, linked both ways.

This repository is the public **install feed**. It distributes the ready-to-install plugin zip and nothing else. **No source code is published here** — Folio is developed in a separate private repository.

- **Download:** grab `folio.zip` from the [Releases page](https://github.com/kristinaquinones/folio-releases/releases).
- **No GitHub account required.** Releases are public; anyone can download.

> **Status:** no release has been published yet. This repository is the destination that Folio's build publishes to, and it is being set up ahead of the first package. There is nothing to download from the Releases page until that lands.

---

## What is Folio?

Folio gives a visual artist two connected surfaces on their own WordPress site.

The **Gallery** is a custom post type for artwork. Each piece carries a museum label — medium, dimensions, year — an availability status, and a short note from the artist. It hangs as a masonry grid, a horizontal scrolling strip, or a slideshow.

The **Journal** uses ordinary WordPress posts, where an entry is the writing behind a particular work. The two are linked in both directions: the artwork page offers the entry, and the journal shows the work each entry is about.

Folio draws the front end for the pages it owns — the gallery, artwork, the journal, its entries, and the About page. Everything else on the site stays with the theme, and deactivating Folio gives all of it back.

---

## Requirements

- Self-hosted WordPress 6.7 or newer, on a site where you can upload plugins or place files in `wp-content/plugins/`.
- PHP 7.4 or newer.
- Any theme. Folio does not require a particular one and does not change the one you have.

---

## Install

1. Download **`folio.zip`** from the [Releases page](https://github.com/kristinaquinones/folio-releases/releases).
2. In wp-admin: **Plugins → Add New → Upload Plugin**.
3. Choose `folio.zip`, click **Install Now**, then **Activate**.

Folio opens on its own welcome screen and walks you through the first few steps from there.

---

## Upgrade

### Manual zip upload

Download a newer `folio.zip` and upload it the same way — **Plugins → Add New → Upload Plugin**. WordPress replaces the plugin folder. Your artwork, journal entries, images, settings, and the links between them are all in the database and are untouched by an upgrade.

After uploading, check the **Plugins** screen: the version shown should match the release you downloaded.

### From the dashboard

*Not available yet.* A future release adds an optional **check this repository for updates** setting, off by default. Until then, upgrading is the manual zip upload above.

When it ships it will be opt-in for a reason worth stating: an update check is an outbound request from your site to GitHub, and whether your site makes it should be your decision rather than a default someone else chose.

---

## Version scheme

- **Stable releases** — clean semver, e.g. `v1.0.0`. Published as normal releases.
- **Pre-releases** — build-stamped `v1.0.0.{build}`, cut automatically as the development line moves. Marked as pre-release on GitHub, and intended for testing rather than for a site anybody visits.

See the [changelog](CHANGELOG.md) for what is in each notable build.

---

## What happens if you remove Folio

Deactivating stops Folio drawing your front end, and your theme takes over again immediately.

Uninstalling removes Folio's own settings and its caches, and nothing else. Every artwork, every journal post, every image, and every link between them stays in your database.

---

## License

Folio is free software, released under the **[GNU General Public License, version 2 or later](LICENSE)** — the same license WordPress itself uses. You may use it, study it, change it, and pass it on. The full terms are in [`LICENSE`](LICENSE) here and bundled inside every `folio.zip`.

---

Copyright © Kristina Quinones
