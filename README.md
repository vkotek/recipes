# Vojtovo Cookbook

A modern plant-based recipe collection and interactive kitchen companion powered by GitHub Pages and Jekyll. Each recipe is a Markdown file in `_recipes/`. The landing page features full-text search, category & tag filtering, nutrition badges, and saved favorites; selecting a recipe opens a two-column kitchen workspace with interactive cooking tools.

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
2. Simmer for 30 minutes until tender.

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

- **Full-text search, sorting & filtering:** Search across titles, categories, tags, descriptions, and full recipe contents (press `/` anywhere to focus search). Combine with quick category pills, multi-tag filters, and sorting by title, protein, calories, or servings.
- **Grid & List views + Saved Favorites:** Switch between editorial cards and a compact list view, bookmark favorite recipes locally, or use **Surprise me** to pick a random dish.
- **Light & Dark themes:** Warm artisanal parchment light mode and roasted espresso dark mode, respecting system preferences with a manual toggle.
- **Two-column kitchen workspace:** Keeps ingredients and equipment in a sticky sidebar alongside numbered method steps on desktop.
- **Interactive checkboxes & progress tracking:** Tap or click any ingredient or method step to check it off and track completion progress in the toolbar.
- **Portion multiplier (`0.5×`, `1×`, `2×`, `3×`):** Automatically scales ingredient quantities and serving counts.
- **Inline step timers:** Automatically detects cooking durations in method steps and lets you launch a floating countdown timer with audio chime.
- **Cook Mode:** Uses the Screen Wake Lock API to keep your screen awake while increasing step legibility for reading from across the counter.

## Publish with GitHub Pages

In the repository, open **Settings → Pages**, choose **Deploy from a branch**, select `main` and the `/ (root)` folder, then save. GitHub Pages will build the Jekyll site from the root of the repository.
