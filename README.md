# RA0SMS Blog

Personal blog about amateur radio, electronics, and RF engineering.

Built with [SkunkHTML](https://github.com/mg0x7BE/skunk-html) — a static blog generator that converts Markdown to HTML via GitHub Actions.

## How to publish a new post

1. Create a Markdown file in the `markdown-blog/` folder.
2. Name the file with the publication date — for example: `2026-07-12.md`
3. Start the file with a `# Title` heading — this becomes the post title.
4. Write the content in Markdown below the title.
5. Commit and push to GitHub. GitHub Actions will automatically build and deploy the site.

### Example

```markdown
# My first QSO on 20m

Today I made my first contact on the 20-meter band...

The band conditions were excellent, I managed to work...
```

### Post with images

Place images in `markdown-blog/images/` and reference them in Markdown:

```markdown
![Antenna description](images/my-antenna.jpg)
```

### Other pages (not blog posts)

If the filename does **not** start with a digit, it becomes a regular page (like `about.md` or `projects.md`). Add a link to it in `html/header.html`.

## Local development

```bash
dotnet restore
dotnet run
```

The site will be generated in the `skunk-html-output/` directory.