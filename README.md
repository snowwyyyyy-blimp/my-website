# My Website

A simple landing page hosted with [GitHub Pages](https://pages.github.com/).

## Features

- Clean, responsive design (HTML/CSS/JS)
- Smooth scrolling navigation
- L4D2 game server status banner from [MantaScope](https://mantascope.com)

## Local preview

Open `index.html` in your browser, or serve it locally:

```bash
# With Python 3
python -m http.server 8000

# With Node (npx serve)
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g., `my-website`).
2. Push this folder to the `main` branch:

   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

3. In the repo on GitHub, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/`.

## The badge

The MantaScope server badge is located in `index.html` inside the `#server` section:

```html
<a href="https://mantascope.com/l4d2/server/gaming-32-players-chaos-2492566?ref=badge">
  <img src="https://mantascope.com/server-img?id=2492566&size=banner&style=console&color=auto"
       srcset="..."
       width="560" height="95" alt="gaming | 32 PLAYERS CHAOS" />
</a>
```