# E-Commerce Odoo Project

Odoo 19.0 addons for the online store: product multi-linking and a set of
`website_sale` extensions (checkout, pricing, stock display, product
matrix, wishlist, and more).

## Running locally

This repo is a set of addon modules, not a standalone app — it needs to be
mounted into an Odoo 19.0 server. The included `docker-compose.yml` (one
level up, in the parent folder) starts Postgres + Odoo with this folder
already wired in as `/mnt/extra-addons`:

```
docker compose up -d
```

Then open http://localhost:8069, create a database, and enable the modules
you need from Apps.

## Licenses

This repository is licensed under [AGPL-3.0](LICENSE).

Each module may carry its own license — check the `license` key in that
module's `__manifest__.py` before redistributing or modifying it.
