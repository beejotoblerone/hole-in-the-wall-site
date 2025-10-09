# Copilot Instructions for AI Agents

## Project Overview
This is an Astro-based static site starter template with a minimal, accessible, and themeable architecture. The project is organized for clarity and rapid prototyping, with a focus on reusable components and global styling.

## Architecture & Key Patterns
- **Astro Framework**: Pages are defined in `src/pages/` (e.g., `index.astro`). Each `.astro` or `.md` file in this folder becomes a route.
- **Components**: Custom UI elements live in `src/components/`. Examples include `Container.astro`, `SkipLink.astro`, and `PropCard.astro`. Components are imported and composed within pages and layouts.
- **Layouts**: Shared page structure is handled in `src/layouts/` (e.g., `Layout.astro`).
- **Global Styles**: CSS resets and theming are managed in `src/content/global/` (`CSSReset.astro`, `Theme.astro`). Use CSS variables for theming.
- **Assets**: Images and other static files are stored in `src/assets/` and `public/`.
- **Import Aliases**: Use `@components`, `@layouts`, `@assets`, and `@content` for cleaner imports (configured in Astro).

## Developer Workflow
- **Install dependencies**: `npm install`
- **Start dev server**: `npm run dev` (default: http://localhost:4321)
- **Build for production**: `npm run build` (output: `./dist/`)
- **Preview build**: `npm run preview`
- **Astro CLI**: Use `npm run astro ...` for commands like `astro add`, `astro check`, etc.

## Project-Specific Conventions
- **Accessibility**: Use `<SkipLink>` for skip navigation. Center content with `<Container>`.
- **Theming**: Use CSS variables in `Theme.astro` for color and style customization.
- **Font Integration**: Fonts are managed via npm (see `@fontsource/karla` in `package.json`).
- **Minimal Boilerplate**: Only essential files and components are included; add features as needed.

## Integration Points
- **External Dependencies**: Astro and `@fontsource/karla` are the main dependencies. Add others via npm as needed.
- **Static Assets**: Place images in `src/assets/images/` or `public/` for direct referencing.

## Examples
- Import a component: `import Container from '@components/Container.astro'`
- Use a layout: `import Layout from '@layouts/Layout.astro'`
- Reference an image: `<img src="@assets/images/logo.png" alt="Logo" />`

## References
- Key files: `src/pages/index.astro`, `src/components/Container.astro`, `src/layouts/Layout.astro`, `src/content/global/Theme.astro`
- For more details, see `README.md` and Astro documentation: https://docs.astro.build

---
If any conventions or workflows are unclear, please ask for clarification or examples from the codebase.
