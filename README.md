# Trump's Dumb Dump of the Day 🇺🇸

An automated fact-checking and media watchdog dashboard tracking the dumbest, most absurd, or blatantly false statements made by Donald Trump in the past 24 hours. Styled using the official **America.gov** design system and vetted against primary transcripts, 3 independent sources, and cross-media framing.

## Project Structure

```text
├── index.html           # Modern, responsive web frontend (Dark mode, Tailwind, Lucide)
├── data/
│   └── quotes.json      # Structured JSON database updated daily by the automated pipeline
├── fetch_daily.py       # Automated ingestion & fact-checking script template
└── README.md            # Setup and deployment documentation
```

## How to View the Website

You can simply open `index.html` in any browser:
- Double click `index.html` in your file explorer, or
- Start a simple local server in this directory:
  ```powershell
  python -m http.server 8000
  ```
  Then navigate to `http://localhost:8000`.

## The 3-Source Fact-Check Rule
To ensure maximum factual accuracy and prevent hallucinations or fake viral quotes:
1. **Primary Verbatim Record**: Speeches, rally transcripts (e.g. Factba.se), or verified Truth Social posts.
2. **Independent Fact-Checker**: PolitiFact, FactCheck.org, or AP Fact Check.
3. **Corroborating Reporting / Primary Source**: Local newspapers, corporate announcements, or government databases.

## Media Framing Analysis
Every daily entry compares two perspectives:
- **Critical / Mainstream**: Highlights factual contradictions and historical records (NPR, NYT, MSNBC).
- **Conservative / Campaign PR**: Highlights how right-wing outlets (Fox News, Sky News, campaign releases) defend or contextualize the rhetoric.
