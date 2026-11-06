# Converge — Faculty Edition

A browser game that teaches faculty to **brief a team of AI helpers** instead of chatting with one. You write a brief for a teaching task; simulated helpers read it once, with nobody to ask, and fill every gap with their own guess. A clear brief makes them converge; a vague one makes them drift apart.

**Play it:** `https://<your-github-username>.github.io/<repository-name>/`

No account, no AI model, no network calls. Everything runs in the player's browser, and progress is saved only in that browser.

---

## Three ways in

Every question set opens with a choice. Players can switch at any time from the board.

| Way in | What happens | Who it suits |
|---|---|---|
| **Just watch** | Each task plays itself: four briefs, from a first try to one that converges, with a caption on what changed and why the helpers moved. No typing. | Anyone meeting the idea for the first time, or who prefers to see before doing. |
| **Guided** | One question at a time. Each shows what the helpers would guess if it were left blank. Your answers become the brief, which you can edit before sending. | Faculty who want structure while they learn what a good brief contains. |
| **Open** | The full game: a blank brief, up to three revisions, credits from tier 3, and a campaign meter. | Curious early adopters and anyone ready for the sandbox. |

Just watch and Guided never change the Open campaign or unlock its tiers.

## What's inside

- **Course content design** (faculty set): a module outline, a reading list with real sources only, notes from your own slides, a discussion-prompt bank, accessible course files, and a syllabus update against a policy memo. Scenarios rotate across biology, history, nursing, teacher education, English and business at an unnamed university. Nothing in the game is any institution's policy.
- **Everyday, Ambient Gen X, Swiftie**: the original warm-up sets.
- **Four tiers**: one helper → three helpers → the swarm (seven agents) → the harness (a fill-in brief the swarm runs without you).
- **Practice and Theory** pages: best practices for briefing AI agents, and the research and pedagogy behind the game.

## A note for facilitators

The alignment score is a pattern match on words. It can be gamed by listing the right terms. **Do not grade people on the number.** Use it as a conversation starter: read the brief, look at the readback beside it, and talk about which decisions the brief made and which it left to the helpers.

---

## Publishing on GitHub Pages

This folder is the finished website. It contains:

```
index.html     the game
assets/        the game's script and styles (keep the folder name and file names exactly as they are)
README.md      this page
```

1. On GitHub, create a new **public** repository (for example `converge-faculty`).
2. Choose **uploading an existing file**, then drag in `index.html`, `README.md` and the whole `assets` folder. Commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set *Source* to **Deploy from a branch**, choose **main** and **/ (root)**, and save.
4. After a minute or two, the address appears at the top of that Settings page. Paste it into the *Play it* line above.

To embed it in Canvas, use that address in an iframe or as an external link.

### Updating later

Each new build produces new file names in `assets/`. When you upload an updated version, delete the old files in `assets/` first, then upload the new `index.html` and `assets` together. Otherwise the page may load the old version.

---

## Credits and licence

- **Original game and engine:** John Courie, who gave permission to adapt and publish it.
- **Faculty edition:** Marybeth ([mbmissenda](https://github.com/mbmissenda)): the Course content design set, the Just watch and Guided ways in, and faculty-focused examples.

The source code (TypeScript, with 87 automated checks including a human-ranked calibration test for every task) is kept separately. Ask the maintainer for the source package to add question sets or make changes.
