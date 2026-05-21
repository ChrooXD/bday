# Siiri's birthday site

## Adding photos

Drop your photos into the `images/` folder and name them `1.jpg` through `8.jpg`.

```
images/
  1.jpg   wide photo — top left, spans 2 columns
  2.jpg   tall photo — right column, spans 2 rows (works best as a portrait)
  3.jpg   square
  4.jpg   square
  5.jpg   wide — spans 2 columns
  6.jpg   square
  7.jpg   square
  8.jpg   wide — bottom right, spans 2 columns
```

Any slot without a matching file just shows as a warm cream block — the grid won't break.

Photos can be `.jpg`, `.jpeg`, or `.png` — just rename them to match the numbered slots.

## Changing the song

Open `index.html` and find this line near the bottom:

```js
const YOUTUBE_ID = 'sXHDC6yEDYU';
```

Replace `sXHDC6yEDYU` with the YouTube video ID you want (the part after `?v=` in the URL). The song plays hidden in the background and loops.

## Deploying to GitHub Pages

1. Create a new **public** repository on GitHub (e.g. `siiri-birthday`)
2. In this folder, run:

```
git init
git add .
git commit -m "birthday site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/siiri-birthday.git
git push -u origin main
```

3. Go to the repo on GitHub → **Settings** → **Pages**
4. Under *Branch*, select `main` and folder `/root`, then click **Save**
5. GitHub will give you a URL like `https://your-username.github.io/siiri-birthday/`

The site is live at that link — send it to Siiri.
