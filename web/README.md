# NLW Agents

A modern web application built with React, Vite, Tailwind CSS, and shadcn/ui.

## Tech Stack

- **React**: UI library for building interactive interfaces.
- **Vite**: Fast build tool and development server.
- **TypeScript**: Type-safe JavaScript.
- **Tailwind CSS**: Utility-first CSS framework.
- **shadcn/ui**: Reusable, accessible React components built on top of Radix UI and Tailwind CSS.
- **React Router DOM**: Routing for React apps.
- **React Query**: Data fetching and caching.
- **Biome**: Code formatting and linting.

## Project Structure & Patterns

- **src/pages/**: Page components (route-based structure).
- **src/lib/**: Utility functions.
- **src/app.tsx & src/main.tsx**: App entry points.
- **shadcn/ui**: Used for building UI components with consistent design and accessibility.
- **Alias**: Use `@/` to import from `src/` (configured in `vite.config.ts` and `tsconfig.json`).

## Setup & Configuration

1. **Install dependencies:**

   ```bash
   npm install
   ```

2. **Development server:**

   ```bash
   npm run dev
   ```

3. **Build for production:**

   ```bash
   npm run build
   ```

4. **Preview production build:**

   ```bash
   npm run preview
   ```

5. **Code style & linting:**

   - Uses [Biome](https://biomejs.dev/) (configured in `biome.jsonc`).
   - Run formatting/linting via Biome CLI if needed.

6. **Tailwind CSS:**
   - Configured via Vite plugin.
   - Use utility classes in your components.

## Notes

- Uses strict TypeScript settings.
- Path alias `@/` for cleaner imports.
- Minimal, modern stack for rapid development.
