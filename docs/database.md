# Data and persistence

There is no database. Orders, customers, machine records, and statuses are stored in repository fixtures such as `src/userdata.js`, `src/constants/customerdata.json`, and machine constants.

This is deterministic for UI development but unsuitable for operational data. A future persistence layer should define identifiers, authorization, audit events, retention, deletion, and migrations before real records are connected.
