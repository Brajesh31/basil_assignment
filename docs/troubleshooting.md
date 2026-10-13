# Troubleshooting

## Dependencies fail to install

Use a supported Node.js version and rerun `npm ci`. Keep the lockfile authoritative.

## The order route is blank

Confirm that `order_id` exists in the local fixture data. The current detail page assumes a matching record and does not yet provide a complete not-found state.

## Refreshing a detail URL returns 404

Configure the static host to rewrite unknown routes to `index.html`; the browser router handles route selection client-side.

## Build or test warnings appear

Run `npm test` and `npm run build` from the repository root and inspect the first reported source file.
