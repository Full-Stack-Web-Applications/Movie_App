# Movie App

A movie browser built with React and React Router on top of the TMDB API.
Browse trending titles, search by name, and open detail pages with nested
cast and reviews views.

**[Live demo](https://goit-react-hw-05-sepia-zeta.vercel.app)**

<img width="1103" height="661" alt="SCR-20261011-bcmn" src="https://github.com/user-attachments/assets/db28de02-093d-42d1-a823-1312d6f29305" />

## Features

- Trending movies of the day
- Search by title
- Movie detail page with nested `cast` and `reviews` routes
- Scroll-to-top control

## Routes

| Path | Page |
|---|---|
| `/` | Trending movies |
| `/movies` | Search |
| `/movie/:id` | Movie details |
| `/movie/:id/cast` | Cast (nested) |
| `/movie/:id/reviews` | Reviews (nested) |

## Tech stack

React 19 · React Router · Vite · Axios · CSS Modules · ESLint

## Getting started

```bash
git clone https://github.com/Full-Stack-Web-Applications/Movie_App.git
cd Movie_App
cp .env.example .env.local    # add your TMDB read access token
npm install
npm run dev
```

Requires Node.js 20.19+ (check the Vite docs for the exact range).
Get a token at https://www.themoviedb.org/settings/api.

## Configuration

| Variable | Description |
|---|---|
| `VITE_TMDB_TOKEN` | TMDB API read access token |

`VITE_` variables are embedded in the client bundle, so the token is visible
in the deployed app. A production version would proxy TMDB requests through a
serverless function.

## Limitations and next steps

- No automated tests yet (planned: Vitest + React Testing Library)
- [Loading/error states: verify and describe]
- Accessibility and performance audits pending

## Credits

This product uses the TMDB API but is not endorsed or certified by TMDB.

## License

MIT
