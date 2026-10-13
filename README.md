# Dota 2 Counter Picker: deploy on Render (free static site)

Files: `index.html` (the whole app), `render.yaml` (Render blueprint).

## Deploy
1. Create a new GitHub repository and upload these files (index.html, render.yaml).
2. Go to https://dashboard.render.com, click **New +**, then **Static Site**.
3. Connect the GitHub repo. Leave **Build Command** empty (or `echo ok`) and set **Publish Directory** to `.`
   (Or choose **New + > Blueprint** and point it at the repo; it reads render.yaml.)
4. Click **Create Static Site**. After about a minute you get a URL like https://dota2-counter-picker.onrender.com

## Notes
- The AI draft engine only works inside Claude. On Render the app runs on the built-in formula and your
  counterpick guide (hard counters), which need no server.
- Hero icons you load are stored in your browser only.
