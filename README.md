# Options Tracker

A personal options-trading journal: dashboard, trade log, and rationale notes,
with broker CSV import and position reconciliation.

## Features

- **Dashboard** — P&L, win rate, open positions, and strategy mix at a glance
- **Trades** — full log with search/filter, opened either manually or by
  importing broker fill CSVs (fills are reconciled into positions, not just
  logged 1:1)
- **Journal** — freeform notes tied to a trade
- Auth and data scoped per user via Supabase

## Stack

React 19 + TypeScript + Vite, React Router, TanStack Query, Supabase
(Postgres + auth), plain CSS (design tokens in `src/styles/nocturne.css`).

## Development

```
npm install
npm run dev       # vite dev server
npm run build     # tsc -b && vite build
npm run lint       # tsc --noEmit
```

Supabase schema/migrations live in `supabase/migrations/`. See
`docs/README.md` for the original UI design spec.
