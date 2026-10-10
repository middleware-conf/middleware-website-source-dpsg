# middleware-website-source-dpsg
Source for https://middleware-conf.github.io (published from
`middleware-conf/middleware-conf.github.io`).

## Updating the site

1. Edit the Markdown files in `content/` (home page: `content/_index.md`).
   The menu is in `config.toml`; give an entry `parent = "<identifier>"` to
   show it in a drop-down under that item (see the Award Winners entries). When you change a page, also update the
   `date:` line at its top; it is shown on the page as the date it was updated.
2. Build with [Hugo 0.128.2](https://github.com/gohugoio/hugo/releases/tag/v0.128.2)
   by running `hugo` in this directory. The theme is vendored in
   `themes/mainroad`; the output goes to `public/`.
3. Commit and push this repo, then copy the contents of `public/` into
   `middleware-conf.github.io` and push that repo (branch `master`).
