# Ayush Kanodia's Personal Website

This repository contains the source code for my personal website, built using Jekyll and the Minimal Mistakes theme.

## Prerequisites

Before you can run this website locally, you need to have the following software installed:

- [Ruby](https://www.ruby-lang.org/en/documentation/installation/) (version 2.5.0 or higher)
- [RubyGems](https://rubygems.org/pages/download)
- [Bundler](https://bundler.io/) (`gem install bundler`)
- [Git](https://git-scm.com/downloads)

## Setup and Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/kanodiaayush/kanodiaayush.github.io.git
   cd kanodiaayush.github.io
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

## Running the Website Locally

To run the website locally for testing and development:

```bash
bundle exec jekyll serve
```

This will start a local web server. You can access the website by opening a browser and navigating to:
```
http://localhost:4000
```

Use the `--livereload` option to automatically refresh the page when you make changes:
```bash
bundle exec jekyll serve --livereload
```

## Building the Website

To build the website without serving it:

```bash
bundle exec jekyll build
```

This will generate the static website in the `_site` directory.

## Adding New Content

### Blog Posts
- Create new blog posts in the `_posts` directory with the filename format: `YYYY-MM-DD-title.md`
- Make sure to include the front matter at the top of each file (see existing posts for examples)

### Pages
- Add new pages to the `_pages` directory
- Update the navigation in `_data/navigation.yml` if needed

## Deployment

This website is automatically deployed to GitHub Pages when changes are pushed to the main branch.

## License

See the [LICENSE](LICENSE) file for details. 

## Known Issues

When building the site, you may see Sass deprecation warnings. These come from the Minimal Mistakes theme and don't affect site functionality. They're related to:
- Deprecated color functions
- Division syntax that will change in Dart Sass 2.0
- CSS declaration placement

These can be safely ignored until the theme is updated. 