# Getting Started with the Data Science Education Portal

This is a simplified version of the Data Science Education Portal using Jekyll with a Feeling Responsive theme approach.

## Installation

You may encounter issues with Ruby 3.4+ and Jekyll due to dependencies. To fix this:

1. Make sure you have Ruby installed
2. Install dependencies:

```bash
gem install bundler
bundle install
```

Ruby 3.4+ has moved some standard libraries out of the default gems. The Gemfile includes:
- `csv` - Required for Ruby 3.4+
- `logger` - Required for future Ruby versions
- `base64` - Required for Ruby 3.4+

If you encounter additional dependency errors, you may need to add those gems to the Gemfile as well.

## Running the Site

To run the site locally:

```bash
bundle exec jekyll serve
```

Then visit http://localhost:4000 in your browser.

## Directory Structure

- `_posts/` - Blog posts with tutorials and articles
- `pages/` - Static pages for different sections
- `assets/` - Images, CSS, and JavaScript assets

## Working with the Site

### Creating New Blog Posts

Add new posts to the `_posts` directory using the naming format `YYYY-MM-DD-title.md`. For example:

```
---
layout: page
title: "Your Post Title"
date: 2025-05-15
teaser: "A brief description of your post"
categories:
    - tutorials
tags:
    - python
    - data-analysis
---

Your post content here...
```

### Adding Images

Place images in the `assets/img` directory and reference them in your content:

```
![Image description](/assets/img/your-image.jpg)
```

## Customization

This site uses a simplified approach to the Feeling Responsive theme. You can customize:

1. The theme by modifying `_config.yml`
2. The homepage layout in `index.html`
3. The navigation in `_config.yml` under "navigation" section