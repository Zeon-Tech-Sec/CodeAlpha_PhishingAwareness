# CodeAlpha_PhishingAwareness

An interactive phishing awareness training module, built for CodeAlpha Cyber Security Internship Task 2.
Open `index.html` in any browser. No install, no server, no dependencies.

Live version (GitHub Pages): https://zeon-tech-sec.github.io/CodeAlpha_PhishingAwareness/

## What is inside

- A "Spot the fake" game: four pairs of sender addresses, tap the fake one and see why (lookalike letters, hidden domains)
- The main phishing types (email, spear phishing, smishing, vishing, business email compromise, quishing) and six red flags
- Six social engineering levers: urgency, authority, fear, reward, curiosity, familiarity
- An interactive inbox test with six emails (four phishing, two legitimate), a link inspector, explanations and a score
- Three real cases: RSA (2011), the Google and Facebook invoice fraud (2013 to 2015) and the Twitter breach (2020)
- Best practices and a checklist for what to do after a click

## Design

Each section is a full-screen flat colour chapter, set in one typeface (Chillax, loaded from Fontshare with a system fallback). The page respects reduced-motion settings and works without JavaScript for reading.

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` directly also works.

## Edit the quiz

The emails are the `mails` array at the bottom of `index.html`. Each entry has `from`, `sub`, `body`, `link`, `href`, `phish` (true or false) and `why`. Add an entry to add a question.

## Notes

All domains in the examples use the reserved `.example` suffix, so none of them point to real sites. This is training material only.
