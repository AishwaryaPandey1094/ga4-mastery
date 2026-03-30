# GA4 Mastery — Free Interactive Flashcard App

Master Google Analytics 4, measurement strategy, attribution, incrementality, and Marketing Mix Modeling with 200+ interactive flashcards.

## Features

- **209 curated questions** across 8 categories and 4 difficulty levels
- **Interactive flip cards** with tap-to-answer and detailed explanations
- **Smart difficulty progression** from Beginner to Expert
- **Category filtering** to focus on weak areas
- **Score tracking** with streaks and accuracy metrics
- **Leaderboard** to track your best performances
- **Social sharing** to share your scores
- **Mobile-responsive** dark-mode design
- **Zero cost** — no API keys, no backend, fully static

## Categories

| Category | Questions | Topics Covered |
|----------|-----------|----------------|
| GA4 Fundamentals | 50 | Event model, data streams, BigQuery, explorations, identity resolution |
| Events & Tracking | 33 | Event types, parameters, GTM, DebugView, Measurement Protocol |
| Attribution & Reporting | 30 | DDA, attribution scopes, segments, engagement metrics |
| Privacy & Consent | 18 | Consent Mode v2, enhanced conversions, GDPR/CCPA |
| Incrementality & Conversion Lift | 23 | Test/control, iROAS, Bayesian methodology, lift types |
| MMM & Meridian | 18 | Bayesian inference, adstock, mROI, budget optimization |
| Google Ads Integration | 18 | gclid, auto-tagging, audiences, conversion discrepancies |
| Role Application (RPL) | 19 | One-to-many enablement, train-the-trainer, portfolio prioritization |

## Difficulty Levels

- **Beginner**: Core concepts, definitions, basic feature identification
- **Intermediate**: Scenario-based application, understanding WHY things work
- **Advanced**: Edge cases, diagnostics, strategic decisions
- **Expert**: Complex multi-concept scenarios, strategic tradeoffs

## Quick Deploy to GitHub Pages

1. **Fork or clone this repo**
2. **Go to Settings → Pages**
3. **Source**: Deploy from a branch → `main` → `/ (root)`
4. **Save** — your site will be live at `https://yourusername.github.io/ga4-mastery/`

## Local Development

Just open `index.html` in a browser. No build step required.

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/ga4-mastery.git
cd ga4-mastery

# Serve locally (Python)
python3 -m http.server 8000

# Or use Node
npx serve .
```

## File Structure

```
ga4-mastery/
├── index.html          # The full app (React loaded from CDN)
├── questions.json      # Question bank (209 questions)
└── README.md           # This file
```

## Adding Questions

Edit `questions.json`. Each question follows this format:

```json
{
  "id": 0,
  "q": "Your question text",
  "o": ["Option A", "Option B", "Option C", "Option D"],
  "c": 1,
  "x": "Explanation of why B is correct",
  "cat": "GA4 Fundamentals",
  "d": 0
}
```

- `c`: Zero-indexed correct answer (0=A, 1=B, 2=C, 3=D)
- `cat`: Must be one of the 8 categories listed above
- `d`: Difficulty level (0=Beginner, 1=Intermediate, 2=Advanced, 3=Expert)

## Built For

This app was originally built for Google Regional Product Lead (Media Effectiveness) interview preparation, covering the measurement concepts and GA4 knowledge required for the role. It is useful for anyone preparing for:

- GA4 Certification exam
- Google measurement and analytics roles
- Digital marketing measurement strategy
- Media effectiveness and attribution analysis

## License

MIT — Free to use, modify, and share.
