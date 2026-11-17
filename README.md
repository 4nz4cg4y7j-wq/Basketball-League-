# League Hub

A website for a 24-team fantasy league with:

- schedule and score entry
- standings
- an automatic Game of the Week
- graphics you can post
- a live 16-team ACC-style playoff bracket
- a playoff predictor

## Put it online (GitHub Pages, free)

1. Create a new **public** repository on GitHub, for example `league-hub`.
2. Add `index.html` and this `README.md`. Use **Add file → Upload files**, or **Add file → Create new file**, name it `index.html` and paste in the contents.
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Pick the branch `main` and the folder `/ (root)`, then click **Save**.
4. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/league-hub/`.

Until you add your own data, the site shows a sample league.

## Updating the league (commissioner)

1. Open the site and go to **Setup**. Enter your league name, your 24 team names and the number of regular-season weeks. Then make a schedule automatically, or paste your Fantrax schedule (one game per line: `week, team, team` or `week, team, score, team, score`).
2. Enter scores under **Schedule & scores**, and playoff scores under **Playoffs**. Your changes save in your browser as you go.
3. Tap **Download data.json**.
4. In your repository, use **Add file → Upload files** to upload `data.json`. If one is already there, it gets replaced. Then commit.
5. Within about a minute, everyone who opens the site sees the update.

Other people can type in the site too, but their changes stay in their own browser. Only the `data.json` in the repository is what everyone sees.

## Fantrax

Fantrax strips out scripts, so the live site can't run inside Fantrax. Instead:

- Post the site's link on your Fantrax league page.
- Under **Playoffs → Put it on Fantrax**, copy the code for the bracket, standings or Game of the Week. Paste it into the HTML/source view of a Fantrax league message. Copy it again after each update, since it's a snapshot.
