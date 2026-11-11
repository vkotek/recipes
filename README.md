# Recipes

A simple recipe collection displayed with GitHub Pages and Jekyll. Each recipe is a Markdown file in `_recipes/`. The landing page shows searchable summaries; selecting a recipe opens its full recipe page.

## Add a recipe

Create a Markdown file in `_recipes/`, for example `_recipes/vegetable-soup.md`:

```markdown
---
title: Vegetable soup
description: A hearty soup with seasonal vegetables.
category: Dinner
tags:
  - vegetarian
  - soup
servings: 4
prep_time: 10 minutes
cook_time: 30 minutes
---

### Ingredients

- 1 onion
- 2 carrots

### Method

1. Chop the vegetables.
2. Simmer until tender.
```

The `title` is required. `description`, `category`, `tags`, `servings`, `prep_time`, and `cook_time` are optional. Search checks titles, categories, tags, and descriptions. Use the tag buttons to include recipes with all selected tags. The full Markdown recipe opens on its own page.

## Publish with GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and the `/ (root)` folder, then save. GitHub Pages will build the Jekyll site from the root of the repository.
