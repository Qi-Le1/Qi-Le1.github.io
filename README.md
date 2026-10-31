# Qi Le's personal website

Site URL: https://qi-le1.github.io/

This Jekyll site uses the AcademicPages theme. The owner authorized republishing the website on 2026-10-31. GitHub Pages publishes the repository's `master` branch from `/` (root), and automatic branch publishing is enabled.

## Update content

- `_pages/about.md`: research profile, project highlights, and recognition.
- `_data/publications.yml`: full author lists, primary paper links, code, venues, and publication status.
- `_pages/publications.html`: publication list rendered from the data file.
- `_pages/service.md`: formal reviewing and faculty co-reviewing, listed separately.
- `assets/Curriculum_Vitae.pdf`: downloadable CV.
- `_config.yml`: profile, links, site metadata, and excluded template examples.
- `_data/navigation.yml`: site navigation.

Keep submitted manuscripts and preprints marked with their actual status. Do not add reviewer years that have not been confirmed.

## Preview

With a current Ruby installation and Bundler:

```sh
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000. Check home, publications, CV, and service at desktop and mobile widths before publishing.

## Publish

Commit reviewed source changes and push to `master` to trigger an automatic GitHub Pages build and deployment. Verify the build and live pages after publishing. Never copy private review reports or other graduate-school records into this repository.

The older Hugo source from Downloads is preserved separately in `../original-materials/`; it is not part of this public repository. AcademicPages/Minimal Mistakes licenses and attribution remain in the source.
