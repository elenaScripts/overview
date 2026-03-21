# Overview

A personal portfolio and blog website built with Hugo static site generator, showcasing technical writing work and documentation samples.

## About

This is the personal website of a technical writer specializing in software documentation and APIs. The site features a portfolio of documentation projects, writing samples, and information about technical writing services.

## Features

- 🎨 Custom homepage with hero section, about me, featured work, and contact sections
- 📝 Blog functionality with Hugo's content management
- 📂 Sample documentation pages showcasing various writing styles
- 🎯 Built with the `hello-friend-ng` Hugo theme
- 🎨 Custom CSS styling for enhanced visual presentation
- 🌐 Multi-language support (English)
- 📱 Responsive design
- 🔍 SEO-friendly structure with sitemap and metadata

## Technology Stack

- **Static Site Generator**: [Hugo](https://gohugo.io/)
- **Theme**: [hello-friend-ng](https://github.com/rhazdon/hugo-theme-hello-friend-ng)
- **Content Format**: Markdown
- **Styling**: Custom CSS

## Prerequisites

- [Hugo](https://gohugo.io/installation/) installed on your system
- Git (for cloning the repository)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd overview
```

2. Install Hugo (if not already installed):
```bash
# macOS
brew install hugo

# Or download from https://gohugo.io/installation/
```

3. Install the theme (if not already included):
```bash
git submodule update --init --recursive
```

## Usage

### Development Server

Run the development server to preview the site locally:

```bash
hugo server
```

The site will be available at `http://localhost:1313`

### Build for Production

Generate static files for deployment:

```bash
hugo
```

The generated files will be in the `public/` directory.

### Create New Content

Create a new post:
```bash
hugo new posts/my-new-post.md
```

Create a new page:
```bash
hugo new about/my-page.md
```

## Project Structure

```
overview/
├── archetypes/          # Content templates
├── content/             # Site content (markdown files)
│   ├── about/          # About page
│   └── samples/        # Documentation samples
├── layouts/             # Custom HTML templates
│   └── partials/       # Reusable template components
├── public/              # Generated static site (gitignored)
├── resources/           # Generated resources cache
├── themes/              # Hugo themes
│   ├── ananke/
│   └── hello-friend-ng/
├── custom.css           # Custom stylesheet
├── hugo.toml           # Hugo configuration file
└── README.md           # This file
```

## Configuration

The main configuration is in `hugo.toml`. Key settings include:

- **Theme**: `hello-friend-ng`
- **Base URL**: Configured for localhost (update for production)
- **Language**: English (en-us)
- **Taxonomies**: Categories, tags, and series
- **Menu**: Home and Samples pages

To customize the site, edit `hugo.toml` and the content files in the `content/` directory.

## Content

The site includes:

- **Homepage**: Custom layout showcasing portfolio and contact information
- **About Page**: Personal information and background
- **Samples**: Documentation samples including:
  - API documentation
  - API reference guides
  - Tutorials and how-to guides
  - Concept documentation
  - Troubleshooting guides
  - And more

## Customization

### Styling

Custom styles are defined in `custom.css`. The homepage uses custom CSS for:
- Hero section styling
- Button designs
- Section layouts
- Contact information formatting

### Layouts

Custom layouts are in the `layouts/` directory. The main homepage layout is in `layouts/index.html`.

## Deployment

The `public/` directory contains the generated static site that can be deployed to:

- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

Simply deploy the contents of the `public/` directory after running `hugo`.

---

Built with ❤️ using [Hugo](https://gohugo.io/)
