# S.T.O.P Online Piracy Response Simulator V1

Static stakeholder-awareness game built with HTML, CSS, vanilla JavaScript and JSON.

## Features
- 40 scenarios across eight learning categories
- Multiple-choice decisions and immediate feedback
- Randomised scenario and answer order
- Score, progress and learning report
- Answer review after completion
- Responsive mobile and desktop interface
- No database, account, backend or AI API
- No links to S.T.O.P IP Trivia

## Files
- `index.html`: page structure
- `style.css`: design and responsive layout
- `app.js`: game logic
- `scenarios.json`: 40 scenarios and explanations

## Run locally
Run `python -m http.server 8000` in this folder and open `http://localhost:8000`. Do not open `index.html` directly via `file://`; browsers often block JSON fetching from local files.

## GitHub + Netlify
1. Create a GitHub repository and upload the project files.
2. Import the repository into Netlify.
3. Leave the build command blank.
4. Set the publish directory to the repository root (`.`).
5. Deploy. Future GitHub pushes trigger redeployment.

## Edit scenarios
Edit `scenarios.json`. Each scenario has `id`, `category`, `title`, `briefing`, `options` and `lesson`. Each option has `text`, `correct` and `feedback`. Exactly one option per scenario must have `correct: true`. V1 expects exactly 40 scenarios; update validation in `app.js` if the total changes.

## Content review
This is general awareness, not legal advice or an official finding of infringement. NCC/S.T.O.P should review legal wording and reporting instructions before public launch. Do not add confidential investigation procedures or sensitive operational information.

## Limitations
Scores remain in the current browser session. V1 has no central score records, user accounts, facilitator dashboard or formal certification.
