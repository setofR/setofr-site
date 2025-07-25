# [ setofℝ ]

My attempt at a personal website. Built with Astro and Tailwind CSS.

## Features

- Home Page
- Blog
- Projects

## Technologies

- [ ] Astro Framework
- [ ] Tailwind CSS
- [ ] Cloudflare
- [ ] JavaScript
- [ ] Markdown

## Project Structure

```
/
├── components/
│   ├── BlogPost.astro
│   └── Project.astro
├── data/
│   └── projects.js
├── layouts/
│   ├── Layout.astro         # base layout
│   └── PostLayout.astro
├── pages/
│   ├── blog.astro
│   ├── index.astro         # home page
│   ├── links.astro         # basically a linktree
│   ├── projects.astro
│   ├── posts/             # post using md file
│   └── tags/              # tag pages
└── styles/
    ├── colors.css         # colour palette
    └── global.css         # needs to be more organised
```

## 📝 Usage

### Blog Post Format

Create a new markdown file in `pages/posts/` directory with the following frontmatter:

```markdown
---
layout: ../../layouts/PostLayout.astro
title: "Your Post Title"
pubDate: MM-DD-YYYY
description: "Brief description of your post"
tags: ["tag1", "tag2"]
---

post stuff here...
```

### Project Format

Edit `data/projects.js` to add a new project

```javascript
{
  title: "Project Name",
  description: "Project description",
  url: "https://github.com/username/repo",
  technologies: ["Tech1", "Tech2"],
  status: "Live", // or "In Progress", "Learning", etc.
  featured: true,
  image: "/path/to/image.jpg" // optional
}
```

### Color Scheme

Edit `styles/colors.css`

```css
:root {
  --color-bg: #000000; /* Background color */
  --color-heading: #ffffff; /* Heading text color */
  --color-text: #cccccc; /* Body text color */
  --color-accent: #808080; /* Accent color */
  --color-border: #333333; /* Border color */
  --color-primary: #808080; /* Primary action color */
}
```

## 📄 License

This project is licensed under the [GPL-3.0 license](LICENSE).

---

⭐ If you found this project helpful, please consider giving it a star!
