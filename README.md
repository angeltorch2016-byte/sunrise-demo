# Sunrise Africa Properties — Investor & Sales Portal (Demo)

A single-file, static, interactive demo built to pitch Sunrise Africa Properties
Limited on a full property sales, investor and realtor platform. No build step,
no backend, no real payments — everything runs client-side so it can be
deployed as-is.

## What's inside
- **Public site** — hero, trust/audit section, filterable property catalogue
  (Ibeju-Lekki, Eleko, Abuja, Ikorodu), a "Digital Operating Layer"
  architecture section (Public → Sales → Transaction → Investor → Trust →
  Management), diaspora-investor section, about, and a contact/enquiry form.
- **Property detail modal** — Overview, **Transparency Centre** (completion
  ring, verified milestone-by-milestone progress table, latest GPS-tagged
  site update with photo/video counts), **Project Passport** (developer,
  legal checklist, financial summary, one-pager style), an interactive site
  plan (click a unit to see live status/price), floor plans, inspection
  booking (date + time slot), and a simulated reservation payment flow
  (Paystack/Flutterwave-style).
- **Investor Portal** (demo login, credentials pre-filled) — dashboard,
  portfolio, payment schedule, documents (allocation letters/receipts),
  site-progress photos, support.
- **Realtor Hub** (demo login) — leads pipeline (kanban), commission tracker,
  promo materials.
- **Developer Command Centre** (demo login via "Command Centre") — portfolio,
  sales and investor stats across every development, a per-project
  completion table, and a sales pipeline funnel.

All data is mock/in-memory JavaScript — refreshing the page resets it.

## Deploy to Vercel
**Option A — Vercel dashboard (no CLI needed)**
1. Go to vercel.com → New Project → Deploy without a Git repo ("Upload" /
   drag-and-drop option), or push this folder to a new GitHub repo and
   import it in Vercel.
2. Framework preset: **Other** (no build command, no output directory needed
   — `index.html` is served as-is).
3. Deploy. Vercel will give you a `*.vercel.app` URL to share with the client.

**Option B — Vercel CLI**
```bash
npm i -g vercel
cd sunrise-demo
vercel --prod
```

No environment variables, dependencies, or build step are required.

## Notes for the pitch
- Colour palette (navy `#0F1B2E`, amber `#D9822C`, cream `#FAF8F3`) was pulled
  from your pitch deck screenshots — the live sunriseafricaproperties.com
  site blocks automated crawling, so it wasn't fetched directly. Worth a
  quick manual check against the real site before the client call.
- Property names, prices, and unit counts are illustrative placeholders —
  swap in real listings before using this beyond the pitch.
