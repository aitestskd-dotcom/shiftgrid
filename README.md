# ShiftGrid (working name)

Invite-only industrial workforce booking and readiness platform for the UAE.

**Status:** pre-product, pre-revenue. No customers, no funding, no government endorsement. All data in the prototype is simulated.

## What it does
Contractors book verified workforce capacity by the hour, week or month through licensed staffing providers. Workers join by invitation, control who sees their profile, and can see pay terms, recorded hours and the pay date before and after each assignment.

## Principles
- Licensed providers remain the legal employers.
- Workers are never charged.
- Customer payment risk must not become worker wage risk.
- Credentials carry a source label: declared, provider-confirmed or issuer-verified.
- No sale of identifiable worker data. No public ratings or blacklists.

## Run the prototype
[Open ShiftGrid prototype](https://aitestskd-dotcom.github.io/shiftgrid/prototype/)

Or run it locally: open `prototype/index.html` in a browser, or serve the folder:

```
cd prototype && python3 -m http.server 8080
```

Flow: Request (match and shortlist) > Readiness (checklist per worker) > Worker view (consent and visibility) > Timesheets (hours rules, approval, wage trail) > Insights.

State is stored in your browser (localStorage). Use Reset in the header to clear it.

## Docs
- docs/product-brief.md
- docs/data-model.md
- docs/compliance-notes.md
- docs/roadmap.md

## Not legal advice
The hours and overtime rules in the prototype are illustrative and need UAE legal review before any production use.
