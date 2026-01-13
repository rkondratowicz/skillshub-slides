# Slidev Kainos Theme

A custom Slidev theme for creating professional presentations.

## Prerequisites

- **Node.js** 18.0.0 or higher
- **npm** or **pnpm** or **yarn**

## Getting Started

### Installation

Install the project dependencies:

```bash
npm install
```

### Development

Start the development server with hot reload:

```bash
npm run dev
```

This will:
- Start a local development server
- Open your presentation in the browser
- Auto-reload when you make changes to slides

### Creating Presentations

1. Create a new Markdown file (e.g., `my-presentation.md`) or edit `example.md`
2. Start with the required frontmatter:

```markdown
---
theme: ./
layout: cover
---

# Your Presentation Title
Your subtitle

---
layout: default
---

# First Slide
Your content here
```

3. Use the available layouts:
   - `cover` - For the opening slide
   - `default` - For regular content slides
   - `end` - For the closing slide

### Available Scripts

- `npm run dev` - Start development server with example.md
- `npm run build` - Build the presentation for production
- `npm run export` - Export presentation to PDF
- `npm run screenshot` - Export slides as PNG images

## Project Structure

```
.
├── assets/          # Static assets (images, etc.)
├── components/      # Vue components
├── layouts/         # Slide layouts
│   ├── cover.vue    # Opening slide layout
│   ├── default.vue  # Default content layout
│   └── end.vue      # Closing slide layout
├── public/          # Public static files
│   └── fonts/       # Custom fonts
├── setup/           # Configuration files
│   └── shiki.ts     # Syntax highlighting config
├── styles/          # Theme styles
│   ├── index.ts
│   └── layout.css
├── example.md       # Example presentation
└── package.json     # Project configuration
```

## Writing Guidelines

- **Start** every presentation with the `cover` layout
- **End** every presentation with the `end` layout
- Define layouts inside the YAML frontmatter (between `---` markers)
- Keep slides concise - maximum 30 words per slide (excluding code)
- Use `<v-clicks>` for progressive content reveal

## Learn More

- [Slidev Documentation](https://sli.dev/)
- [Slidev Theme Guide](https://sli.dev/guide/write-theme.html)
- [Why Slidev?](https://sli.dev/guide/why)

## Font Configuration

This theme uses:
- **Sans-serif**: Century Gothic
- **Monospace**: Fira Code

Fonts are configured in package.json and should be placed in `public/fonts/`.
