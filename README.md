# Yuyang Hu - Academic Website

Personal academic website built with [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## Local Development

1. Install Ruby and Bundler (if not already installed)
2. Run:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
3. Open http://localhost:4000

## Deploy to GitHub Pages

To deploy at `https://Hu-Yuyang.github.io`:

1. Create a new repository named `Hu-Yuyang.github.io` on GitHub (or use "Use this template" from al-folio)
2. Push this project to the repository:
   ```bash
   cd al-folio-website
   git remote set-url origin https://github.com/Hu-Yuyang/Hu-Yuyang.github.io.git
   git add .
   git commit -m "Initial commit: Yuyang Hu academic website"
   git push -u origin main
   ```
3. In repository Settings → Pages: set source to "GitHub Actions" (or "Deploy from branch" with gh-pages)
4. The site will build and deploy automatically

## Content Overview

- **About**: Bio, profile, selected publications, news
- **Publications**: Auto-generated from `_bibliography/papers.bib`
- **Projects**: Research projects (KDS, Cloud Removal, Implicit Priors, SPICER)
- **CV**: PDF at `/assets/pdf/YuyangHu_CV.pdf`
- **News**: Announcements and updates

## Customization

- Edit `_config.yml` for site-wide settings
- Edit `_pages/about.md` for biography
- Add publications to `_bibliography/papers.bib`
- Add projects to `_projects/`
- Add news to `_news/`
- Social links: `_data/socials.yml`
