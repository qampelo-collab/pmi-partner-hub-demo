# PMI Enterprise Partner Hub — prototype

A closed B2B portal where an enterprise customer discovers, buys and manages everything PMI
offers, and where the people inside that organisation manage their own development against it.

**Live: https://qampelo-collab.github.io/pmi-partner-hub-demo/**

One self-contained HTML file. No framework, no build step, no external request — it works
offline from a double-click, and the live URL is the same file.

---

## What this is, and what it is not

A representation of a **desired customer experience** and the capability set behind it. It is
**not a proposed technical solution** and not an argument to build. Roughly half of what it
shows is standard B2B platform capability that several commercial products already provide;
a smaller set is genuinely PMI's. The in-product **capability map** sorts all 34 capabilities
into buy, configure or build, and into three delivery waves.

Every figure, price, name and organisation in here is **invented**. Northwind Industries and
Meridian Systems are fictional. Nothing in this artefact is PMI list pricing or a PMI
commercial term.

Open **About this prototype** in the hub for the full position, including a Q&A.

## What is in the current version

Three plans and six profiles, all in one file — switch with the control in the header:

| Plan | Profile | Who that is |
|---|---|---|
| Enterprise | Platform Administrator | Runs the hub: access, seats, orders, audit |
| Enterprise | Capability Manager | A division director; their people and a delegated budget |
| Enterprise | Capability Sponsor | Owns the outcome and the money |
| Enterprise | Billing Contact | Accounts payable; invoices and nothing else |
| Business | Business Account Owner | A 50–300 person company buying for itself |
| Either | Learner | The individual |

The substance: two assessments that turn the catalogue into a ranked shortlist, a commercial
layer with budgets, purchase orders and delegated authority, a full billing and invoicing
surface, the demand loop that scores an individual's request against the organisation's own
assessed gaps, six illustrated role guides, and the capability map.

## Review mode

`index.html` carries an optional review layer. **It is off by default** — the hub opens as the
product. The switch in the header (or the `R` key) turns it on; then every section carries a
comment button, and comments get a verdict, an importance, a name and a timestamp.

Comments live in the reviewer's own browser. There is no server, so consolidating several
reviewers is explicit: each exports a JSON file from the review board, and one person imports
them there. **How to review**, in the hub's Review menu, explains the whole loop.

**The link to send a reviewer** turns the layer on and starts them on the instructions:

    https://qampelo-collab.github.io/pmi-partner-hub-demo/?review=1

The plain URL above stays the product — it opens on the dashboard and says nothing about
reviewing unless somebody reaches for the switch.

## Files

| Path | What it is |
|---|---|
| `index.html` | **The current build.** What the live URL serves. Includes the review layer, off by default. |
| `versions/v6.html` | The same product without the review layer. |
| `versions/v4.2.html` | Three admin roles, organisation structure, escalation. |
| `versions/v4.html` | Assessments, commercial layer, learner access model. |
| `versions/v3.html` | The base shell every later version is composed from. |
| `versions/v2.html` | Catalogue and admin console. |
| `versions/v1.html` | The first prototype. |

Older versions are kept so a change can be traced, not because they are maintained. Only
`index.html` is current.

Any version can be opened directly, e.g.
`https://qampelo-collab.github.io/pmi-partner-hub-demo/versions/v6.html`
