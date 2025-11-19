# AI Copilot Instructions for clone-tabnews

## Project Overview

**clone-tabnews** is a learning project built with Next.js to understand web development fundamentals through the curso.dev course. It's a minimal React/Next.js application with code style enforcement.

- **Framework**: Next.js 13+ with React 18
- **Language**: JavaScript (not TypeScript)
- **Node Version**: LTS/Hydrogen (specified in `.nvmrc`)
- **Code Style**: Prettier (2-space indentation via `.editorconfig`)

## Architecture & Key Files

This is a **Next.js Pages Router** application (not App Router):
- **`pages/index.js`** - Main homepage component; exports a default React component
  - Currently contains two components: `Home` (h1) and `TextDecoderStream` (h2)
  - Components are defined at file-level, not using standard Next.js page conventions

**No backend, API routes, or database** - this is a static frontend learning project.

## Development Workflow

| Task | Command |
|------|---------|
| Start dev server | `npm run dev` (runs `next dev`) |
| Check code formatting | `npm run lint:check` (prettier --check) |
| Fix code formatting | `npm run lint:fix` (prettier --write) |

## Code Style & Conventions

- **Formatting**: Prettier-enforced with 2-space indentation
- **React**: Functional components only; no class components
- **JavaScript**: Vanilla JS (no TypeScript at this stage)
- **File Structure**: Components at page level in `pages/` directory
- **Exports**: Always use `export default` for page components

When modifying `pages/index.js`:
1. Ensure components are functional (arrow functions or function declarations)
2. Run `npm run lint:fix` before committing
3. Don't introduce TypeScript or external component libraries not in `package.json`

## Important Notes for Agents

- This is an **educational project** - prioritize clarity and simplicity over optimization
- No tests or CI/CD pipelines exist; focus on core functionality
- Dependencies are minimal: only Next.js, React, React-DOM, and Prettier
- If adding features, check `package.json` to avoid suggesting missing dependencies
- Portuguese language is used in component text (educational context from curso.dev)
