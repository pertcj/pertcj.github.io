# pertcj.github.io

Personal academic website for Charles Pert, built on the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template and hosted on GitHub Pages.

## Structure

- `_config.yml`: site-wide settings (name, bio, social links)
- `_pages/about.md`: homepage bio and news
- `_pages/cv.md`: CV page template
- `_data/cv/*.yml`: editable CV sections rendered by `_pages/cv.md`
- `_publications/`: one Markdown file per paper
- `_talks/`: one Markdown file per invited talk
- `_workshops/`: one Markdown file per workshop
- `files/`: downloadable files (e.g., BibTeX entries)
- `images/avatar.jpg`: profile photo

## Updating content

Edit the relevant Markdown file and push to `main`. GitHub Pages rebuilds the site automatically, no local build required.

To add a new publication or talk, copy an existing file in `_publications/` or `_talks/` and update the YAML front matter.

To update the CV, edit the relevant file in `_data/cv/`. The page is rebuilt automatically by Jekyll whenever the site is built.

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
```

Requires Ruby and Bundler. Not required to deploy, GitHub Pages builds the site itself on push.
