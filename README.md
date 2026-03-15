# Maze-Solver-Bot

An interactive maze generation and pathfinding visualizer built with vanilla HTML, CSS, and JavaScript. Visualizes BFS, DFS, and A* algorithms solving randomly generated mazes in real time.

🔗 **Live Demo:** [https://maze-solver-bot.pages.dev/](https://maze-solver-bot.pages.dev/)

---

## Features

- Random maze generation using iterative DFS (recursive backtracker)
- Three pathfinding algorithms: BFS, DFS, A*
- Animated exploration and path tracing
- Random start and end points on every new maze
- Stats panel showing path length, cells explored, and compute time

---

## Algorithms

| Algorithm | Shortest Path | Notes |
|-----------|--------------|-------|
| BFS | ✅ Yes | Explores level by level |
| DFS | ❌ No | Fast, explores deep first |
| A* | ✅ Yes | Uses Manhattan distance heuristic, most efficient |

---

## Project Structure
```
Maze-Solver-Bot/
└── index.html      # Entire app — no dependencies, no build step
```

No `package.json`, no `requirements.txt`, no frameworks. Everything runs in the browser.

---

## Run Locally

Open terminal and navigate to the project folder:
```bash
cd path/to/maze-solver
```

Then open the file directly in your browser:
```bash
start index.html
```

> On Mac use `open index.html` · On Linux use `xdg-open index.html`

---

## Deploy on Cloudflare Pages

### First-time setup

1. Push the project to a GitHub repository
2. Go to [cloudflare.com](https://cloudflare.com) → **Workers & Pages**
3. Click **Create** → **Pages** → **Connect to Git**
4. Select your GitHub repository
5. Under **Build settings** — leave everything blank (no build command, no output directory needed)
6. Click **Save and Deploy**

Your site will be live at `https://your-repo-name.pages.dev`

### Update the live site

Every push to the `main` branch automatically redeploys:
```bash
git add index.html
git commit -m "your update message"
git push
```

Cloudflare detects the push and updates the live site within ~30 seconds.

### Via GitHub website (no terminal)

1. Open your repo on github.com
2. Click `index.html` → click the **pencil (Edit)** icon
3. Paste updated code
4. Click **Commit changes**

Done — Cloudflare Pages redeploys automatically.

---

## No Requirements File Needed

This project has zero dependencies. It runs entirely in the browser using:

- Plain HTML5
- CSS3
- Vanilla JavaScript 

No npm, no pip, no installs required.
