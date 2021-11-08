# futter

## abstract

A simple theme for recipes.

## features

Configure your recipes in the front matter to get a nice readable page and also
a [schema.org recipe](https://schema.org/Recipe) in JSON-LD on top of it.

## example

This is how I did it. Is it the best way? Probably not. Does it work? For now,
yes. If you're unhappy with what you're reading: PR are welcome.

### directory structure

Inside of the `content` directory, things should look like this to work with
futter:

```
.
├── Ramen-Noodles
│   ├── images
│   │   └── ramen.jpeg
│   └── index.md
└── Rosinenbroetchen
    ├── images
    │   └── Rosinenbroetchen.jpeg
    └── index.md
```

### front matter

Content of your posts are also part of the recipe, but the important bits are
gathered from the front matter.

```
---
title: Rosinenbroetchen

recipe:
  totalTime: 10m
  author: Malte
  recipeIngredient:
  - one banana
  - two rosinen
  recipeInstructions:
  - one
  - two
  recipeYield: 2 Teller
  totalTime: 10m
  diet: Fleisch

---

Das weniger fettige Brioche ... mit Rosinen.
```
