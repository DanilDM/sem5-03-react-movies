# React Movies

Movie search app built with React, TypeScript and the [TMDB API](https://www.themoviedb.org/).

**Live demo:** https://sem5-03-react-movies.vercel.app/

## Features

- Search movies by keyword (React 19 Form Actions)
- Movie grid with posters; loader and error states
- Modal with details (backdrop, overview, release date, rating), rendered via `createPortal`
- Modal closes on close button, `Esc` key and backdrop click; body scroll is locked while open
- Toast notifications for empty query and empty results (React Hot Toast)

## Tech stack

- Vite + React 19 + TypeScript
- Axios
- CSS Modules
- modern-normalize
- React Hot Toast
- Prettier

## Project structure

```
src/
├── components/
│   ├── App/
│   ├── ErrorMessage/
│   ├── Loader/
│   ├── MovieGrid/
│   ├── MovieModal/
│   └── SearchBar/
├── services/
│   └── movieService.ts
├── types/
│   └── movie.ts
└── main.tsx
```

Each component folder contains `Component.tsx` and `Component.module.css`.

## Getting started

```bash
git clone https://github.com/<your-username>/03-react-movies.git
cd 03-react-movies
npm install
```

Create a `.env` file in the project root with your TMDB API Read Access Token:

```
VITE_TMDB_TOKEN=your_tmdb_token
```

Run the dev server:

```bash
npm run dev
```

## Scripts

| Command           | Description              |
| ----------------- | ------------------------ |
| `npm run dev`     | Start dev server         |
| `npm run build`   | Type-check and build     |
| `npm run preview` | Preview production build |
| `npm run lint`    | Run ESLint               |

## Deployment

Deployed on Vercel. Set `VITE_TMDB_TOKEN` in **Project Settings → Environment Variables** before deploying.

## Attribution

This product uses the TMDB API but is not endorsed or certified by TMDB.