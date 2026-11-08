# papermood-blog

A ready-to-write blog starter for [Accent CMS](https://accentcms.dev) on
the [Papermood](https://hub.accentcms.dev/themes/papermood) theme: post
cards, a dark-mode toggle, archives, tag pages, client-side search, and a
trilingual interface (English, German, French) with a language switcher.

## Use it

```bash
accent init my-blog --template papermood-blog
cd my-blog
accent serve
```

Then open the URL the server prints. The starter ships with a home card,
an about page, and four example posts that double as documentation: a
getting-started guide, a markdown reference, a note on the dark mode, and
a translated first post that shows the i18n mechanism.

## What to edit first

- `config.yaml` -- the site name, the public URL, and the theme options
  under `site.extra.papermood`.
- `models/default.yaml` -- the site-wide `author` default; every post
  without an `author:` line shows this name.
- `content/home/default.md` (and `.de.md`, `.fr.md`) -- the markdown body
  of the home page fills the intro card, per language.

The vendored theme lives in `themes/papermood`, installed from the hub.
`accent theme update` tracks new releases once you reinstall it from the
registry: `accent theme install papermood`.

## License

MIT. The bundled Papermood theme is MIT as well; its design follows
[hugo-PaperMod](https://github.com/adityatelange/hugo-PaperMod) by
adityatelange and contributors (MIT).
