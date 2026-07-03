# mohammadabh.github.io

Personal academic website for Mohammad Albinhassan, built on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template and hosted on GitHub Pages.

## Structure

- `_config.yml`: site-wide settings (name, bio, social links)
- `_pages/about.md`: homepage bio and news
- `_pages/cv.md`: CV page
- `_publications/`: one Markdown file per paper
- `_talks/`: one Markdown file per invited talk
- `files/`: downloadable PDFs (CV, papers, slides)
- `images/mohammad-profile.jpg`: profile photo

## Updating content

Edit the relevant Markdown file and push to `main`. GitHub Pages rebuilds the site automatically, no local build required.

To add a new publication or talk, copy an existing file in `_publications/` or `_talks/` and update the YAML front matter.

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
```

Requires Ruby and Bundler. Not required to deploy, GitHub Pages builds the site itself on push.
