# ORPAZ-EVENT — Prototype frontend

Version: 0.2.0 — 23 November 2026

## Contents
- `index.html`: storefront structure and modal workflows.
- `styles.css`: responsive luxury visual system.
- `app.js`: language switching (FR/EN/HE/ES), product rendering, category filters, product detail modal, local cart, event lead form and demo interactions.
- `catalogue-bijoux.md`: provenance, imported sample scope and product-data validation caveats.

## Run locally
Open `index.html` in a modern browser. For a local server:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Important implementation status
This is a working frontend prototype, not a production commerce system. The jewelry section now contains 42 sample references transcribed from public Atelier Orpaz collection pages. Prices are observations, not live-synced values; some are starting prices. Product images remain temporary demonstration images. The beauty products remain illustrative. Cart and event enquiry persistence are local to the browser. No real customer account, payment, order management, inventory, email delivery, CRM, tax calculation, shipping provider or booking calendar is connected.

## Production work still required
1. Select and configure the final domain and hosting.
2. Create the Shopify store and connect the real catalog, inventory, checkout and order webhooks.
3. Implement the server-side application and PostgreSQL schema for events, quotes, bookings, partners, permissions and audit logs.
4. Integrate payment provider(s), verified webhooks, deposits, balances, refunds and reconciliation.
5. Implement secure authentication and role-based access control.
6. Implement transactional email, consent management, privacy and legal pages.
7. Connect the official Shopify catalogue/API and sync all variants, prices, availability and product details; replace temporary jewelry images with approved official assets. See `catalogue-bijoux.md` for the exact import scope and caveats.
8. Complete accessibility, security, performance, SEO and end-to-end testing.

## Notes
- The Hebrew locale enables RTL layout at the document level. All components require native-speaker QA before launch.
- No credentials or API secrets are included in this prototype.
