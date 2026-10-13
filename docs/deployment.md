# Deployment

Build the static bundle with `npm ci` followed by `npm run build`, then serve `build/` from a static host configured to return `index.html` for client-side routes, including `/order/:order_id`.

When adding an API, use build-time public configuration only, never embed secrets in `REACT_APP_*` variables, and configure HTTPS, security headers, authenticated API access, and route fallback behavior.
