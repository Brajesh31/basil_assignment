# Contributing

Keep customer and payment data synthetic until a reviewed backend integration exists.

1. Create a focused branch.
2. Install with `npm ci`.
3. Run `npm test` and `npm run build`.
4. Test `/` and `/order/:order_id`, including empty and missing-record states.
5. Update documentation when routes, fixtures, or Redux state change.

Pull requests should describe the affected UI, verification commands, and accessibility or security implications. Report vulnerabilities privately using [SECURITY.md](SECURITY.md).
