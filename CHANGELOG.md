# Changelog

Notable changes to the **Folio** install packages distributed from this repository. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and Folio uses [semantic versioning](https://semver.org/spec/v2.0.0.html).

This is the artist-facing install feed: it summarizes what is in the `folio.zip` you download, not every commit behind it.

- **Stable releases** use plain semver, e.g. `1.0.0`.
- **Pre-releases** are build-stamped `1.0.0.{build}` and carry the current development line. They are for testing.

For every published build, see [Releases](https://github.com/kristinaquinones/folio-releases/releases).

---

## [Unreleased]

The first package. Nothing has been published yet; this section becomes `[1.0.0]` when it is.

### Added

- **Gallery** — artwork as a post type, each piece carrying a museum label (medium, dimensions, year), an availability status, and a note from the artist. Three layouts: masonry grid, horizontal scrolling strip, and slideshow, with the pace of the moving ones as a setting.
- **Journal** — entries written as ordinary WordPress posts, linked to a work in both directions, so the artwork offers its entry and the journal shows the work each entry is about.
- **Curate** — drag or arrow the gallery into the order you want it hung. Sequencing is what a portfolio is, and the order a visitor sees is the order you set.
- **A front end Folio draws itself** for the gallery, artwork, the journal, entries, and the About page. Any theme; nothing switched; deactivating gives it all back.
- **Detail shots** — extra images on a work, shown as a row of squares beneath it, each opening a lightbox scoped to that work.
- **Light and dark**, as a site-wide setting independent of which gallery layout you chose.
- **Your own words in the navigation** — rename Work, Journal, and About, and add your own pages to the nav.
- **Replies on journal entries**, off by default. WordPress keeps deciding how comments behave in Settings → Discussion; Folio's switch only decides whether readers see them.
- **Focus mode**, on by default: the admin shows Folio rather than all of WordPress, without removing anything or blocking any screen.
- **Search that reads the museum label**, so looking for "gouache" finds the work made of it, not only works with it in the title.
- **Accessibility to WCAG 2.1 AA**, including a reduced-motion setting that works alongside the browser's own.

---

[Unreleased]: https://github.com/kristinaquinones/folio-releases/releases
