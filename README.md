# Basil Order Dashboard

Basil Order Dashboard is a React and TypeScript operations interface for browsing machine orders, reviewing order statistics, filtering records, and opening order details. It is a Create React App frontend using Tailwind CSS, Redux Toolkit, React Router, date-range controls, and AG Grid styling.

> **Current scope:** This is a frontend prototype. Orders, customers, machines, and statuses are local fixtures; the refund control is presentation-only and no backend or payment service is connected.

## Features

- Responsive application shell with sidebar and navigation.
- Orders view with statistics, tables, status chips, machine filters, and date filters.
- Order details at `/order/:order_id`.
- Local customer and machine fixture data.
- Redux state for selected filters.

## Getting started

```powershell
npm ci
npm start
```

Open <http://localhost:3000>. The current app needs no database or secret. Available scripts are `npm start`, `npm test`, and `npm run build`.

## Project layout

- `src/App.tsx` - routes and layout composition.
- `src/pages/` - order list and detail views.
- `src/components/` - reusable layout, table, status, and filter components.
- `src/redux/` - Redux store and filter slice.
- `src/constants/` and `src/userdata.js` - local fixture data.

Keep fixture data synthetic. Before connecting customer or payment data, add authenticated API access, authorization, validation, audit logging, and privacy controls. See [SECURITY.md](SECURITY.md).

## License

MIT licensed. See [LICENSE](LICENSE).

Last updated: 2026-10-18 02:00 UTC
