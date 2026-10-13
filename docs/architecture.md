# Architecture

The application is a client-rendered React frontend bootstrapped with Create React App.

`src/App.tsx` creates the browser router and maps `/` to the order dashboard and `/order/:order_id` to order details. `MainLayout` supplies navigation. Shared components provide breadcrumbs, filters, statistics, status chips, and tables.

Redux Toolkit stores filter state in `src/redux/`. Pages read local fixture data from `src/userdata.js` and constants. There is no server API, authentication boundary, persistence service, or payment integration.
