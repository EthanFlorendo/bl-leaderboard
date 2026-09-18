# The Reading League 📚

A leaderboard my friends and I use to track who's reading what.

**Live site:** https://ethanflorendo.github.io/bl-leaderboard/

## What it does

- Tracks books each reader is currently reading, has finished, or has paused
- Shows a leaderboard/stats view so we can see who's ahead
- Lets you sort by date, rating, author, or completion
- Has a planner for books people want to read next
- Admin mode can add, edit, and seed books for everyone

## How it's built

Plain HTML/CSS/JS, no framework or build step,  just static files served straight from GitHub Pages. Data lives in [Supabase](https://supabase.com/), pulled in via their JS client.

```
index.html
src/
  components/   UI bits (navbar, book cards, search, modals, etc.)
  pages/        home, leaderboard, and admin views
  services/     Supabase/auth/books/planner data fetching
  state/        simple app state
  utils/        constants and helpers
```
