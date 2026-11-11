# Recipes

A simple recipe collection displayed with GitHub Pages and Jekyll. Recipes are stored as Markdown files in `_recipes/`; the homepage renders their titles and contents. Use `category` and `tags` in each recipe's front matter to organize and find recipes.

## Add a recipe

Create a Markdown file in `_recipes/`, for example `_recipes/vegetable-soup.md`:

```markdown
---
title: Vegetable soup
category: Dinner
tags:
  - vegetarian
  - soup
prep_time: 10 minutes
cook_time: 30 minutes
---

A short description.

### Ingredients

- 1 onion
- 2 carrots

### Method

1. Chop the vegetables.
2. Simmer until tender.
```

The `title` is required. `category`, `tags`, `prep_time`, and `cook_time` are optional. Search checks recipe text, including ingredients and tags; selecting a tag fills the search field. Categories are available in the category filter. Write recipe content in regular Markdown.

## Publish with GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and the `/ (root)` folder, then save. GitHub Pages will build the Jekyll site from the root of the repository.
