# Recipes

A simple recipe collection displayed with GitHub Pages and Jekyll. Recipes are stored as Markdown files in `_recipes/`; the homepage renders their titles and contents.

## Add a recipe

Create a Markdown file in `_recipes/`, for example `_recipes/vegetable-soup.md`:

```markdown
---
title: Vegetable soup
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

The `title` is required. `prep_time` and `cook_time` are optional. Write the recipe body in regular Markdown; the homepage displays it automatically.

## Publish with GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and the `/ (root)` folder, then save. GitHub Pages will build the Jekyll site from the root of the repository.
