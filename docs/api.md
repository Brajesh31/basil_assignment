# Routes and data contracts

The frontend currently exposes browser routes rather than an HTTP API:

| Route | Purpose |
| --- | --- |
| `/` | Order list, statistics, filters, and navigation shell |
| `/order/:order_id` | Detail view for a matching local fixture |

The detail view expects fields including `order_id`, `status`, `date`, `machine_name`, `total_amount`, `customer_name`, and `contact_number`. A future API should document authentication, pagination, validation, refund idempotency, and errors.
