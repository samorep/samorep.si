# Jekyll GitHub Pages Site

This is a simple GitHub Pages site built with Jekyll.

## Setup

1. Install Ruby and Bundler if you haven't already.
2. Clone this repository.
3. Run `bundle install` to install dependencies.
4. Run `bundle exec jekyll serve` to start the local development server.
5. Visit `http://localhost:4000` to view your site.

## GitHub Pages Configuration

To configure this site to work with GitHub Pages:

1. Replace the `repository` value in `_config.yml` with your GitHub username/repository name.
2. Push your repository to GitHub.
3. Go to your repository's Settings > Pages.
4. Set the source to your main branch.
5. Wait a few minutes for your site to be built and deployed.

## Structure

- `_config.yml`: Site configuration
- `_layouts/`: Layout templates
- `_posts/`: Blog posts
- `assets/`: CSS, JavaScript, and images
- `index.md`: Home page
- `about.md`: About page

## Creating New Posts

Add new posts in the `_posts/` directory following the naming convention `YYYY-MM-DD-title.md`. Each post should have front matter at the top:

```markdown
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS +0000
categories: category1 category2
---
```

## Customization

To customize this site, edit the following files:

- `_config.yml`: Change site title, description, and other settings.
- `_layouts/`: Edit the HTML templates.
- `assets/css/main.scss`: Modify the styling.
- Create new posts in the `_posts/` directory following the filename format `YYYY-MM-DD-title.md`. 