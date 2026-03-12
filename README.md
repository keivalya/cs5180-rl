# CS 5180/4180 Reinforcement Learning Interactive Demos

Interactive, browser-based teaching tools for core reinforcement learning topics from CS 5180/4180.

## Project Structure

This project is a static website. Each chapter/demo is a standalone HTML page:

- `index.html`: Landing page with links to all chapters
- `bandits.html`: Multi-armed bandits
- `mdp.html`: Markov decision processes
- `dp.html`: Dynamic programming
- `mc.html`: Monte Carlo methods
- `mc_es.html`: Monte Carlo ES (Blackjack)
- `td.html`: Temporal-difference learning
- `random_walk.html`: Random walk (TD vs MC)
- `windy_gw.html`: Windy Gridworld (SARSA/Q-learning)
- `n_step_bootstrapping.html`: n-step TD bootstrapping
- `planning_tabular.html`: Dyna-Q planning vs Q-learning
- `eligibility_traces.html`: TD(0) vs TD(lambda), accumulating/replacing traces
- `background-animation.js`: Shared animated background script (used by `index.html`)
- `favicon.svg`: Site icon
- `CNAME`: Custom domain configuration for GitHub Pages

## Run Locally

No build tooling is required.

1. Open `index.html` directly in a browser, or
2. Serve the folder with a lightweight static server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy

This repository is ready for static hosting (for example, GitHub Pages).  
Push changes to the configured branch and the site serves directly from HTML/CSS/JS files.

## Adding a New Demo Page

1. Create a new `*.html` page in the repository root.
2. Keep styles and interaction patterns consistent with existing pages.
3. Add a link card for the page in `index.html`.
4. Verify the page works standalone in a browser.

## Notes

- The project is intentionally framework-free for portability and easy classroom use.
- Most demos render charts and environments using HTML canvas.
