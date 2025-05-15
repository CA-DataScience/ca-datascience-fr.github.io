# Data Science Education Portal

A Jekyll-based website providing educational resources for data science students and educators, built with the Feeling Responsive theme.

## About This Site

This site serves as an educational portal for data science, offering:

- Resources for students learning data science
- Materials for educators teaching data science
- Blog posts on data science concepts and events
- FAQs and common questions about the field

## Technical Details

- Built with Jekyll 4.3+
- Uses the Feeling Responsive theme
- Mobile-friendly and responsive design
- Includes blog functionality

## Running Locally

To run this site locally:

1. Install Jekyll and Bundler:
   ```
   gem install jekyll bundler
   ```

2. Install dependencies:
   ```
   bundle install
   ```

3. Start the Jekyll server:
   ```
   bundle exec jekyll serve
   ```

4. View the site at `http://localhost:4000`

## Adding Content

### Blog Posts

Create a new Markdown file in the `_posts` directory with the naming convention:
```
YYYY-MM-DD-title-with-hyphens.md
```

Include front matter at the top of your post:
```yaml
---
layout: page
title: "Your Post Title"
date: YYYY-MM-DD
teaser: "A short description of the post"
categories:
    - category1
    - category2
tags:
    - tag1
    - tag2
---
```

### Pages

Create new pages in the `pages` directory with appropriate front matter:
```yaml
---
layout: page
title: "Page Title"
permalink: "/page-url/"
header:
  image_fullwidth: header_image.jpg
---
```