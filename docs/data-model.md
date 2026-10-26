# Data model (linked records)

| Record | Purpose | Core fields |
|---|---|---|
| Worker | One worker-controlled profile | worker_id, trade, grade, years, languages, availability_date, last_confirmed, visibility, consent_status |
| Credential | Evidence per worker | credential_type, issuer, number, expiry, source_label (declared, provider-confirmed, issuer-verified) |
| Provider | Licensed employer of record | provider_id, licence_reference, insurance_status |
| Customer | Industrial contractor | customer_id, sites, requirements |
| Request | Demand | request_id, trade, quantity, start, duration, site_requirements |
| Assignment | Worker booked to a request | assignment_id, worker_id, provider_id, request_id, terms |
| Timesheet | Recorded hours | assignment_id, daily_hours, worker_review_status, approval |
| Payment trail | Wage and invoice events | wages_due_date, wages_paid_at, invoice_reconciled_at |

## Rules
- Sensitive attributes (nationality, religion, health, family status) are not searchable.
- Identity documents are stored in an encrypted vault and are never shown to customers.
- Each processing purpose has its own legal basis; one consent checkbox is not used for everything.
- Performance fields are bounded, attributable and challengeable. No cross-employer blacklist.
