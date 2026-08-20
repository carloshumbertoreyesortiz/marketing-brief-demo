# Marketing brief assistant — public demo

A front-end prototype of an AI-assisted intake form for marketing activity requests.

**Live demo:** https://carloshumbertoreyesortiz.github.io/marketing-brief-demo/

## What it does

You describe a marketing activity in your own words on the left. The assistant asks follow-up
questions one at a time — only for what your description did not already cover — and builds a
structured brief on the right as you talk.

- **Seven questions:** audience, company size, resellers, existing products, other characteristics, goal, deadline
- **Three clearance gates:** pricing, product and sales. *"Does this need clearance?"* → *"Has it been done?"* — and **"don't know" blocks submission**
- **Deadline validation:** minimum two weeks ahead, corrected if you pick something earlier
- **Draft output:** a customer-facing email and SMS, which deliberately never mention how the audience was selected
- **On submit:** a structured JSON record plus a readable Markdown rendering

## Try this first

1. Describe any activity, e.g. *"We want to offer a free upgrade to customers who already have Mobile Voice"*
2. Answer the questions as they come
3. At *"Does this activity need clearance with pricing?"* answer **Ja** (yes)
4. At *"Has it been done?"* answer **Vet ikke** (don't know)
5. Try to submit — it refuses, and tells you which area needs clearing

## Notes

- **The AI is simulated.** Extraction is keyword matching, not a language model — it will misread things
- **Fictional throughout.** Northwind Business, Team Connect, Mobile Voice are invented
- **No data leaves your browser.** Everything is `localStorage`; nothing is sent anywhere
- Norwegian by default — use the **EN** toggle in the header for English

Single self-contained page. No build step, no backend.
