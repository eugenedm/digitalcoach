---
layout: post
title: Part 5. WHAT RESULT?
has_children: true
nav_order: 5

---


# What Result? Point B.
{: .no_toc }



CSS utility classes come in handy when you to want to override default styles to create additional whitespace (margins/padding), correct unexpected shifts in font size or weight, add color, or hide (or show) something at a specific screen size.
{: .fs-6 .fw-300 }

---

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## No Problems? No business!

The main navigation for your Just the Docs site is on the left side of the page at large screens and on the top (behind a tap) on small screens. The main navigation can be structured to accommodate a multi-level menu system (pages with children and grandchildren).

---

## From Current to Desired Situation

To specify a page order, use the `nav_order` parameter in your pages' YAML front matter.

---

## First $2,000-$3,000

Sometimes you will want to create a page with many children (a section). First, it is recommended that you keep pages that are related in a directory together... For example, in these docs, we keep all of the written documentation in the `./docs` directory and each of the sections in subdirectories like `./docs/ui-components` and `./docs/utilities`. This gives us an organization like:

```
+-- ..
|-- (Jekyll files)
|
|-- docs
|   |-- ui-components
|   |   |-- index.md  (parent page)
|   |   |-- buttons.md
|   |   |-- code.md
|   |   |-- labels.md
|   |   |-- tables.md
|   |   +-- typography.md
|   |
|   |-- utilities
|   |   |-- index.md      (parent page)
|   |   |-- color.md
|   |   |-- layout.md
|   |   |-- responsive-modifiers.md
|   |   +-- typography.md
|   |
|   |-- (other md files, pages with no children)
|   +-- ..
|
|-- (Jekyll files)
+-- ..
```

On the parent pages, add this YAML front matter parameter:
-  `has_children: true` (tells us that this is a parent page)




This example skips the page name heading (`#`) from the TOC, as well as the heading for the Table of Contents itself (`##`) because it is redundant, followed by the table of contents itself.






![](https://guides.github.com/activities/hello-world/branching.png)

