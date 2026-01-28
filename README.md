# Stylescape Svelte Example

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/stylescape/example-svelte)

Stylescape example using [Svelte](https://svelte.dev/) and [SvelteKit](https://kit.svelte.dev/).

## About Stylescape

Stylescape is a visual identity framework by [Scape Agency](https://www.scape.agency) providing a complete design system with components, layouts, and utilities.

## Features Demonstrated

- Frame layout with `frame_main`
- Top/bottom ribbons
- Collapsible sidebars (`data-ss="aside"`)
- Accordion component (`data-ss="accordion"`)
- Theme toggle (`data-ss="theme-toggle"`)

## Installation

```bash
npm install
```

## Usage

```bash
npm run dev   # Start development server
npm run build # Build for production
```

## Project Structure

```
src/
├── routes/
│   └── +page.svelte
├── app.html
└── scss/
    └── styles.scss
```

## Learn More

- [Stylescape Documentation](https://github.com/stylescape/stylescape)
- [Svelte Documentation](https://svelte.dev/docs)

## License

MIT
