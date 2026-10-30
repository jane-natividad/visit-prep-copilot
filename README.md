# Visit Prep Copilot

A visit-preparation prototype for primary care: reads a synthetic patient record between visits and flags what may need a second look before the next appointment — every flag traced to the record entry behind it.

**[Live demo](https://visit-prep-copilot.vercel.app)** — works immediately, no API key or setup required. Everything runs in your browser; nothing you enter is stored or sent anywhere. Please use fictional/sample data only.

## Who it's for

Family physicians who want to know what's changed since a patient's last visit before they walk in, not reconstruct it from scratch.

## Why it matters

Patients managing an ongoing condition can fall through the gaps between visits — a dose changed by a specialist that never matched what the pharmacy dispensed, a referral sent and never closed — with nobody actively watching to make sure it does. This tool does that watching between visits, so the physician walks in knowing what changed and what to ask, with the receipts attached.

## What it does

- Pick one of three synthetic patients and get a visit-prep view: changes since last visit, prioritized flags, and suggested questions
- Rule-based flags: prescribed vs. dispensed dose mismatches, overdue monitoring, open referrals with no result, abnormal results with no follow-up, risky over-the-counter combinations
- Every flag cites the record entries it came from; a timeline view shows the full record with post-visit entries highlighted
- Physician can mark each flag reviewed or not relevant — the tool never resolves anything on its own

## Product decisions that mattered more than the model

1. **Rules, not a model** — same record in, same flags out, and each rule is readable in the code
2. **Receipts on every flag** — a physician should be able to verify a flag in seconds, not trust it
3. **A quiet record is a valid answer** — the tool says 'nothing flagged' rather than inventing something to show

## Built with

- HTML, CSS, JavaScript (single-file prototype, no framework, no build step)

## Run locally

Open `index.html` in any browser — no install needed.

## Status

This is a prototype built to explore a problem space, using fictional/synthetic data — not a finished product and not connected to any organization's real systems. Built by [Jane Natividad](https://github.com/jane-natividad) — see more at [jane-natividad.github.io](https://jane-natividad.github.io).
