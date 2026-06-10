# Pre-launch checklist

Things to replace in each report HTML before sending to a candidate.

## Per-report (every new candidate)

- [ ] **Candidate name** — appears in `<title>`, `<h1>`, and the score gauge section
- [ ] **Score (66)** — update all `input[value]` fields in the 10 Dimensions section; the gauge calculates from these automatically
- [ ] **Validity date** — the "Report pricing valid until" line in the Pricing section (currently hardcoded as 17 June 2026 — should be report date + 7 days)
- [ ] **Before/After examples** — the 4 `[data-ba]` cards; replace with the candidate's actual resume lines and the rewritten versions
- [ ] **Summary paragraphs** — the 4 cards in "What a recruiter sees in 8 seconds" (Recruiter perception, The problem, ATS risk, Shortlist probability)
- [ ] **Risk cards** — the 5 items in "Why this resume may not get shortlisted"; adjust wording and High/Medium tags to match
- [ ] **Keyword chips** — the 5 keyword groups; add/remove chips based on what's actually missing from this resume
- [ ] **Dimension labels** — the small italic description under each of the 10 dimension rows
- [ ] **Hero verdict pills** — the 4 coloured pills (✓ Good technical depth etc.); update to match the candidate's profile
- [ ] **Locked preview bullets** — the 5 blurred bullet points in "A preview of your rewritten resume"; replace with a real teaser rewrite

## Once (global setup — do these once before any report goes out)

- [ ] **Razorpay payment links** — replace `href="#"` on "Get Resume Pro" and "Get Resume Package" buttons with your actual Razorpay payment page URLs
- [ ] **WhatsApp link** — replace `href="#"` on "Chat with us on WhatsApp" with `https://wa.me/91XXXXXXXXXX`
- [ ] **Callback link** — replace `href="#"` on "request a callback" with your Calendly or typeform link
- [ ] **Social proof numbers** — update the 3 stat boxes (1,200+ resumes, +21 pts, 2–3 days) once you have real data; leave as-is for now if approximate
- [ ] **Testimonials** — replace placeholder quotes with real ones (name, role, city)
- [ ] **Segment snippet** — add your `analytics.load("YOUR_WRITE_KEY")` snippet before `</body>`; all event calls (`analytics.track(...)`) are already wired in the JS

## Optional but recommended

- [ ] **OG meta tags** — add `<meta property="og:title">`, `og:description`, `og:image` so the link previews nicely when shared on WhatsApp
- [ ] **Favicon** — add `<link rel="icon">` pointing to the Talent500 favicon
- [ ] **`<meta name="robots" content="noindex">` on all reports** — you don't want candidate reports indexed by Google
