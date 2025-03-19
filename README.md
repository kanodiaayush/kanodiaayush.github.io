# Ayush Kanodia's Personal Website

This is a Jekyll-based personal website and blog using the minimalist theme with a sunrise color scheme.

## Setup Instructions

1. Make sure you have Ruby and Bundler installed:
   ```
   ruby -v
   gem install bundler
   ```

2. Install the required dependencies:
   ```
   cd jekyll_site
   bundle install
   ```

3. Run the Jekyll server locally:
   ```
   bundle exec jekyll serve
   ```

4. View the site at http://localhost:4000

## Deployment with GitHub Pages

To deploy this site using GitHub Pages:

1. Push this code to the desired branch (e.g., `jekyll` or `main`)
2. In GitHub repository settings, ensure GitHub Pages is enabled and pointing to the correct branch
3. Your site will be available at kanodiaayush.github.io

## Adding New Blog Posts

To add a new blog post, create a new Markdown file in the `_posts` directory following the naming convention:

```
YYYY-MM-DD-title-of-post.md
```

Include the following front matter at the top of your post:

```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
author: Ayush Kanodia
categories: category1 category2
---
```

For posts with mathematical content, add `usemathjax: true` to the front matter.

## Theme and Design

This site uses:
- Jekyll theme: jekyll-theme-minimalist
- Color scheme: sunrise (warm, light colors with orange accents)

## Contact

If you have any questions, feel free to reach out to me through the links on the website. 