# 💍 Proposal Website

A cute, romantic proposal site. She opens an envelope, reads your love story line by line, gets asked "Will you marry me?" (the **No** button runs away 😄), then signs a "Promise of Forever" by typing her name. After that comes a celebration with hearts and confetti, all with your song playing in the background.

## 1. Personalize it
Open `index.html` and edit the `CONFIG` block near the top:

| Setting | What it does |
|---|---|
| `herName` | What you call her (shown on the envelope) |
| `yourName` | Your name (your signature on the proposal) |
| `music` | File name of your song, e.g. `music.mp3` |
| `musicStartAt` | Second to start the song from (e.g. `42` to jump to the chorus) |
| `story` | The lines of your love story. Write as many as you like |
| `promises` | The promises she agrees to when she signs |
| `finalMessage` | The message she sees after she says yes |

## 2. Add your song
Put your song file (MP3 works best) in this folder, next to `index.html`, and name it `music.mp3`. If you use a different name, change `music` in the CONFIG to match.
The music starts when she taps the envelope, because browsers block autoplay until someone taps. A ♫ button in the corner lets her pause it.

## 3. Push to GitHub
```bash
cd proposal
git init
git add .
git commit -m "For her 💍"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```
(Or create a new repo on github.com and upload the files with the "Add file → Upload files" button.)

> Tip: make the repo **private** so she can't stumble on it first.

## 4. Deploy on Vercel
1. Go to https://vercel.com and log in with GitHub.
2. Click **Add New → Project** and import your repo.
3. Framework preset: **Other**. Leave the build settings empty.
4. Click **Deploy**. You'll get a link like `https://your-project.vercel.app`.

Every push to GitHub redeploys the site automatically.

## Before the big moment
- Open the link on **your own phone** first, with the volume up, to test the music and the whole flow.
- To give the link a cuter name, open the project's **Settings → Domains** in Vercel and choose something like `forever-us.vercel.app`.

Good luck! 💖
