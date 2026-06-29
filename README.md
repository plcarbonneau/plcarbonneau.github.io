# Journalism Portfolio (TeXt theme)

This is a [Jekyll](https://jekyllrb.com/) site built on the [TeXt theme](https://github.com/kitian616/jekyll-TeXt-theme), set up as a journalism portfolio with sections for your clips, about page, resume, and contact info. It's ready to deploy on GitHub Pages for free.

## 1. Personalize it

- **`_config.yml`** — search for `TODO` and fill in: your name, bio, email, social handles, GitHub repo path, site URL, and timezone.
- **`about.md`** — your bio, beats, background, awards.
- **`resume.md`** — your work history, education, skills. Optionally drop a PDF at `assets/files/resume.pdf` and it'll link from the top of the page.
- **`contact.md`** — email and social links.
- **`assets/images/avatar.jpg`** — replace the placeholder with a real headshot (square works best).

## 2. Add your clips

Each published story is a "post" in `_posts/`. Three examples are included to show the pattern — duplicate one, then edit:

```
_posts/2026-01-15-example-investigative-story.md
```

Filename format is `YYYY-MM-DD-slug.md` (the date doesn't have to be exact — it just controls sort order). Inside each file:

```yaml
---
title: "Your Real Headline"
tags: Investigations   # used for filtering on the Clips page — pick a category
cover: /assets/images/your-cover.jpg   # add a real thumbnail, or remove this line
---

A short summary of the story and why it matters.

<!--more-->

**Published in:** Outlet Name, Month Year

[Read the full story at Outlet Name →](https://link-to-the-real-article.com)
```

This pattern (summary + link out) is standard for portfolios since the outlet — not you — usually holds rights to the published text. If a piece is unpublished or self-published, you can write the full piece directly in the post body instead.

Delete the three example posts once you've replaced them with real clips.

## 3. Preview it locally (optional)

Requires [Ruby + Bundler](https://www.ruby-lang.org/en/documentation/installation/).

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## 4. Deploy to GitHub Pages

1. Create a new GitHub repo named **`your-username.github.io`** (replace `your-username` with your actual GitHub username) — this gives you a free site at that exact URL with no extra config.
   - If you'd rather use a project repo with any name instead, set `baseurl: "/your-repo-name"` in `_config.yml`.
2. Push this folder's contents to that repo's `main` branch.
3. In the repo on GitHub, go to **Settings → Pages**, and under "Build and deployment" set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**.
4. Wait a minute or two — your site will be live at `https://your-username.github.io`.

## Theme reference

For deeper customization (skins, layouts, comments, analytics, search), see the original [TeXt theme docs](https://kitian616.github.io/jekyll-TeXt-theme/docs/en/quick-start).

Current skin: `dark` (set in `_config.yml` as `text_skin`). Other options: `default`, `forest`, `ocean`, `chocolate`, `orange`.
