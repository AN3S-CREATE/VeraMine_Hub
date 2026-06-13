# AGENTS.md

## Cursor Cloud specific instructions

VeraMine Hub is a single-service, frontend-only app: Vite + React 18 + TypeScript + Tailwind CSS. There is no backend, database, or test suite.

- Dev server: `npm run dev` (Vite, serves on http://localhost:5173/). This is the command to run/preview the app during development.
- Build / typecheck: `npm run build` (runs `tsc` then `vite build`). This is the only "lint-like" gate since there is no separate lint script and no tests.
- Production preview: `npm run preview` (serves the built `dist/`).
- Node 20+ works (CI uses Node 20; the VM has Node 22, which is fine).
- The app is a slide-deck dashboard (`src/App.tsx`); slide navigation is via on-screen chevron buttons.
