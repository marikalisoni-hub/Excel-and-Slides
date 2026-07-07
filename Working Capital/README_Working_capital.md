# Working Capital & Cash Flow Deep-Dive — Read Me

This folder contains a self-directed financial-analysis project: a benchmark of how
efficiently two companies convert their operations into cash, and a quantified set of
actions the weaker performer could take to release cash.

> **Illustrative data.** The two companies — *Alpha Subsea Systems* and *Beta Energy
> Equipment* — are fictional, with synthetic but realistic figures modelled on a
> subsea / energy-equipment business. The purpose is to demonstrate the analytical method
> on a clean dataset, not to report on any real company.

## What's in the folder

**1. `Working_Capital_Deep_Dive.xlsx` — the model**
A four-tab Excel workbook:

- **README** — purpose, definitions, method and sources.
- **Inputs** — the raw financials for both companies (blue = hardcoded input). All
  calculations elsewhere link back here, so changing one number updates the whole model.
- **WC Analysis** — the core comparison. Five ratios, calculated with live formulas (no
  hardcoded numbers): DSO, DIO, DPO, the cash conversion cycle (CCC), and net working
  capital as a % of revenue. It also includes a short methodology memo showing a
  purchases-based DPO alongside the standard COGS-based one.
- **Levers** — three quantified cash-release levers (inventory, payables, receivables),
  each with an editable target, the resulting cash freed, and the trade-off involved.

**2. `Working_Capital_Summary.pptx` — the summary**
A four-slide deck that presents the story: the headline gap between the two companies, why
it exists, where the cash is trapped (broken into the three drivers), and the three levers
with a closing recommendation.

## How to read it

Start with the deck for the story (about two minutes), then open the Excel model to see the
workings. In the model, the flow is **Inputs → WC Analysis → Levers**.

## The five metrics in one line each

- **DSO** — days to collect cash from customers (lower is better).
- **DIO** — days inventory is held before sale (lower is better).
- **DPO** — days taken to pay suppliers (higher means more supplier financing).
- **CCC** — DSO + DIO − DPO; net days cash is tied up (lower is better).
- **NWC %** — receivables + inventory − payables, as a share of revenue.

## Headline finding (illustrative)

On this dataset, Alpha runs a ~143-day cash conversion cycle against Beta's ~34, and ties
up ~36% of revenue in working capital versus ~10%. The gap is driven mainly by inventory,
with slower customer collection and weaker payables terms adding to it. Closing part of the
gap across all three drivers could release roughly $470m (~13% of revenue), split between an
inventory lever, a receivables lever and a payables lever — each with its trade-off stated.

## Method notes

Ratios use period-end balances (a standard screening simplification; a two-point average
would refine them). Because the companies are illustrative, the dollar figures size a prize
rather than describe a real result. A live version of this analysis would use audited
filings and be built bottom-up by product line and supplier segment.
