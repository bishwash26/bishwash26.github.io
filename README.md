# bishwash26.github.io

Personal site + blog. Built with Jekyll, hosted on GitHub Pages (no build step needed on your side — GitHub builds it on every push).

## Go live (one time)

1. On GitHub, create a **public** repo named exactly `bishwash26.github.io`.
2. Push this folder to it:
   ```sh
   cd bishwash26.github.io
   git init && git add . && git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/bishwash26/bishwash26.github.io.git
   git push -u origin main
   ```
3. Repo → **Settings → Pages** → Source: *Deploy from a branch*, Branch: `main` / `(root)`.
4. Wait ~1 minute, then open https://bishwash26.github.io

## Write a post

1. Copy `_drafts/post-template.md` to `_posts/YYYY-MM-DD-some-slug.md`
   (the date in the filename is the publish date; the slug becomes the URL).
2. Fill in the front matter (`title`, `description`, `tags`) and write Markdown.
3. `git add . && git commit -m "post: some slug" && git push` — it's live in about a minute.

Posts in `_drafts/` are never published. Delete or rewrite `_posts/2026-11-15-hello-world.md` (it's a formatting reference).

## Preview locally (optional)

```sh
bundle install
bundle exec jekyll serve --drafts --livereload
# open http://localhost:4000
```

## Where things live

| file | what |
|------|------|
| `index.html` | home page: intro, projects, experience, stack |
| `blog/index.html` | blog listing |
| `_layouts/post.html` | single-post layout |
| `assets/css/main.css` | the whole theme (colors at the top) |
| `_config.yml` | name, links, URL |

Feed is at `/feed.xml`; sitemap and SEO/OG tags are generated automatically.
