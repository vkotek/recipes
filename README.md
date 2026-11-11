# Recipes

A simple recipe collection displayed with GitHub Pages and Jekyll. Each recipe is a Markdown file in `_recipes/`. The landing page shows searchable summaries; selecting a recipe opens its full recipe page, styled by a shared layout.

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
source: https://example.com/vegetable-soup
image: /assets/images/vegetable-soup.jpg
image_alt: A bowl of vegetable soup with fresh herbs
---

### Ingredients

- 1 onion
- 2 carrots

### Method

1. Chop the vegetables.
2. Simmer until tender.

### Nutrition

| Nutrient | Per serving (1/4 of recipe) | Whole recipe (4 servings) |
| :--- | ---: | ---: |
| **Calories** | 120 kcal | 480 kcal |
| **Protein** | 4 g | 16 g |
| **Carbohydrates** | 22 g | 88 g |
| **Fiber** | 5 g | 20 g |
| **Fat** | 2 g | 8 g |
```

The `title` is required. `description`, `category`, `tags`, `servings`, `prep_time`, `cook_time`, `source`, `image`, and `image_alt` are optional. Put recipe photos in `assets/images/` and use a site-root path such as `/assets/images/vegetable-soup.jpg`.

### Features

- **Full-text search & filtering:** Search checks titles, categories, tags, descriptions, and full recipe contents (including ingredients). Combine search with the category dropdown and multi-tag filter buttons.
- **Interactive checkboxes:** Tap or click any ingredient or method step to check it off while cooking.
- **Portion multiplier (`0.5×`, `1×`, `2×`, `3×`):** Automatically scales ingredient quantities and serving counts.
- **Cook Mode:** Uses the Screen Wake Lock API to keep your phone or tablet screen awake while following a recipe.

## Publish with GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and the `/ (root)` folder, then save. GitHub Pages will build the Jekyll site from the root of the repository.
