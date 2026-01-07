# The Mamelodi Initiative Website

This repository contains the Jekyll source code for The Mamelodi Initiative
website, an educational non-profit in South Africa.

**Want to contribute content or report an issue?** Email
[info@mamelodi.org](mailto:info@mamelodi.org) or see the sections below.

## Contributing Content

We welcome contributions of stories, media, and reports from the Mamelodi
Initiative community!

### For Content Creators

If you have content to share but aren't familiar with GitHub, simply email your
submission to [info@mamelodi.org](mailto:info@mamelodi.org) with the following
information:

**For Stories** (student achievements, alumni updates, community impact):
- Publication date
- Story title
- Main content (text)
- Brief excerpt (1-2 sentences, under 160 characters)
- Optional: Photo or image
- Optional: Thumbnail image (approximately 150px wide for list view)

**For Media Posts** (videos and photos):
- Publication date
- Media title
- Brief description or excerpt (1-2 sentences, under 160 characters)
- YouTube or Vimeo video URL (if applicable) - thumbnail will be automatically pulled from the video
- Photos or image files (if applicable)
- Optional: Thumbnail image (approximately 150px wide for list view) - only needed for non-video media

**For Reports** (programme reports, annual reports, evaluations):
- Publication date
- Report title
- Brief excerpt (1-2 sentences, under 160 characters) for list view
- Executive summary (full summary paragraph/section for the report page)
- Full report content (text) or download link (PDF)
- Optional: Tags (e.g., "summer-jam", "winter-jam", "annual-report")

### For Developers

If you're comfortable with GitHub and Jekyll:

1. If you have write access to the repository, create a new branch; otherwise, fork this repository
2. Create a new markdown file in the appropriate `_posts/` subdirectory:
   - `_posts/stories/` for student/community stories
   - `_posts/media/` for photos/videos
   - `_posts/reports/` for programme reports
3. Follow the naming convention: `YYYY-MM-DD-title.md`
4. Use these examples as templates:
   - Stories: [`_posts/stories/2015-05-20-marvin-lukas-segl.md`](_posts/stories/2015-05-20-marvin-lukas-segl.md)
   - Reports: [`_posts/reports/2025-02-04-summer-jam-2025-report.md`](_posts/reports/2025-02-04-summer-jam-2025-report.md)
   - Media: [`_posts/media/2013-07-31-why-education.md`](_posts/media/2013-07-31-why-education.md)
5. Include required front matter: `title`, `date`, `categories`, `excerpt`, and `header.teaser` (defaults may be used); optional: `tags`
6. For video embeds, use: `{% include video id="..." provider="youtube" %}` or `provider="vimeo"`
7. Submit a pull request

See [`AGENTS.md`](AGENTS.md) for detailed technical documentation.

## Development

This is a static site built with [Jekyll](https://jekyllrb.com/) and hosted on
GitHub Pages. It uses the
[Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes) remote theme.

**Note:** For simple post additions, you may not need to run the site locally -
you can create the markdown file and submit a pull request. The markdown changes
will be reviewable in the PR, though the rendered site won't be visible until
after merging.

### Running Locally

If you already have Ruby and Bundler installed:
```bash
bundle install
bundle exec jekyll serve --livereload
```

If you're new to Jekyll, you'll first need to install Ruby (2.7+) and Bundler.
See the [Jekyll installation guide](https://jekyllrb.com/docs/installation/) for
platform-specific instructions.

## Issues

Found a bug or have a suggestion? You can:
- Email us at [info@mamelodi.org](mailto:info@mamelodi.org)
- Create a [GitHub issue](https://github.com/mamelodi/mamelodi.github.io/issues)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Some layout files in `_includes/` are derived from the Minimal Mistakes theme, which is also MIT licensed.
