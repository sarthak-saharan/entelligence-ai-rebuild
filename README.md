# Entelligence AI — Interactive Demo Prototype

A self-contained interactive demo page for [Entelligence AI](https://entelligence.ai), built to pitch a **conversion rate improvement** to their founders.

🔗 **Live demo:** [sarthak-saharan.github.io/entelligence-ai-rebuild](https://sarthak-saharan.github.io/entelligence-ai-rebuild)

---

## What this is

The current Entelligence homepage shows only static screenshots. High-intent engineers want to *feel* the product before signing up. This prototype adds:

1. **Role-based quiz** — asks the visitor their role (EM, Senior Eng, CTO, PM, Scrum Master, Security Eng) and one contextual follow-up question, then personalises the entire demo experience around their specific pain points.

2. **Interactive "Try Ellie" demo** — simulates Ellie's adversarial code review loop with:
   - 3 pre-built code snippets (Connection Leak, Auth Bypass, Race Condition)
   - A live "paste your own code" tab with in-browser pattern detection
   - Typewriter-style AI reasoning animation with variable timing
   - Animated diff view when "Apply fix in one click" is clicked

3. **Personalized end CTA** — "That's 1% of what Ellie can do for Engineering Managers" with role-specific feature callouts and a "Book a 20-min demo" button.

---

## Design constraints

Matches Entelligence's exact design system:

| Token | Value |
|-------|-------|
| Accent color | `#444d36` (olive) |
| Font | Inter / system-ui |
| Dark panel bg | `#171717` |
| Card bg | `#1e1e1e` |
| Button radius | `14px` |
| Card radius | `16px` |

- No external JS dependencies — single self-contained HTML file
- Ellie mascot image embedded as base64 (no external image requests)
- Google Fonts (Inter) is the only external resource

---

## File structure

```
index.html          # The prototype (single file, self-contained)
ellie-demo.html     # Same file, original name
Ellie.png           # Ellie mascot source image
README.md
```

---

## Hosting

Served via GitHub Pages from the `main` branch root. Any push to `main` updates the live URL automatically.

---

## Local development

```bash
python3 -m http.server 5173
# open http://localhost:5173
```
