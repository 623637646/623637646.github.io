# 623637646.github.io

My blog, built with [Zola](https://www.getzola.org) and the [tabi](https://github.com/welpo/tabi)
theme, and deployed to GitHub Pages by `.github/workflows/deploy.yml` on every push to `master`.

```bash
git clone --recurse-submodules git@github.com:623637646/623637646.github.io.git
zola serve --drafts   # http://127.0.0.1:1111, not localhost: the theme's CSP allows only its own origin
```

A post is a folder in `content/blog/` with an `index.md`, and `index.zh-Hans.md` for its Chinese
version. `draft = true` in its front matter keeps it out of the published site.
