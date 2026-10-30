# Visit Prep Copilot

Shows a physician what changed since the last visit, and what might need a second look.

**[Try the live demo](https://visit-prep-copilot.vercel.app)**. It works straight away with no setup, runs entirely in your browser, and stores nothing. All data is fictional or synthetic.

## Why I built it

This grew out of a primary care product I've been building. Talking with family physicians, I kept hearing how much time goes into reconstructing what happened since the last visit. This version runs on synthetic patients so anyone can try it in a browser.

## The problem

Patients managing an ongoing condition can fall through the gaps between visits: a dose changed by a specialist that never matched what the pharmacy dispensed, or a referral that was sent and never closed.

## What I built

A visit preparation view that reads a synthetic patient record and lists what changed, what may need attention and a few questions worth asking. Every flag shows the record entries it came from, and only the physician can mark it reviewed.

## Who it's for

Family physicians who want to know what's changed before they walk into the room.

## What it does

- Choose one of three synthetic patients and see changes since the last visit, prioritized flags and suggested questions
- Flags dose mismatches, overdue monitoring, open referrals, abnormal results without follow up and risky over the counter combinations
- Cites the record entries behind every flag, with a full timeline view
- Lets the physician mark each flag reviewed or not relevant

## Decisions that shaped it

1. **Clear rules:** the same record always gives the same flags.
2. **Receipts on every flag:** a physician can check any flag in seconds.
3. **A quiet record is a good answer:** it only raises what's genuinely there.

## Key takeaway

It supports clinical review and leaves diagnosis and treatment to the physician. Every flag traces back to the record.

## Built with

- HTML, CSS and JavaScript in a single file

## Run it locally

Open `index.html` in any browser. There's nothing to install.

## About this project

This is a working prototype I built to explore a real problem space. It uses illustrative, fictional data and isn't connected to any organisation's systems. You can find more of my work at [jane-natividad.github.io](https://jane-natividad.github.io).

Built by [Jane Natividad](https://github.com/jane-natividad).
