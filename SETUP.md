# How to install your new profile README

Your profile README lives in a special repo named after your username. Follow these steps.

## 1. Create (or open) the special repo

- Make a **public** repo named exactly **`Sophie-S-Z`** — same as your username. GitHub will show a note: "You found a secret! Sophie-S-Z/Sophie-S-Z is a special repository..."
- If it already exists, just edit it.

## 2. Add the files

Put these at the repo root:

```
Sophie-S-Z/
├── README.md            ← the profile file
├── assets/
│   └── dachshund.svg    ← your custom trotting dachshund
└── .github/
    └── workflows/
        └── snake.yml    ← OPTIONAL, only if you want the contribution-eating animation
```

- **README.md** → repo root
- **dachshund.svg** → inside an `assets/` folder
- **snake.yml** → inside `.github/workflows/` (rename it to `snake.yml` there)

## 3. The dachshund

The README already points to `assets/dachshund.svg` on your `main` branch. It's a hand-built
animated SVG (a real "eats your grid" wiener-dog action doesn't exist off the shelf, so this is
a cute decorative stand-in that trots across on loop). It animates on GitHub with no setup — just
commit it.

If your default branch is `master` instead of `main`, change the image URL in README.md from
`/main/` to `/master/`.

## 4. Optional — the real contribution-grid animation

If you also want the classic snake that eats your actual contribution squares:

1. Add `.github/workflows/snake.yml`.
2. Go to the repo's **Actions** tab → run **"Generate Snake"** once (workflow_dispatch).
3. It creates an `output` branch with the SVGs. Then add this to README.md where you like:

```markdown
![Snake](https://raw.githubusercontent.com/Sophie-S-Z/Sophie-S-Z/output/github-snake-dark.svg)
```

It refreshes every 12 hours automatically.

## 5. Things to personalize (marked in the README with `EDIT` comments)

- **Typing header text** — change the `lines=` part of the demolab URL.
- **"What I'm up to" / "Featured projects"** — swap in whatever you're actually shipping right now. The one blank I left: a one-line description of **Noema** (I didn't know what it is).
- **Tech stack badges** — remove anything you don't use, add what you do. Browse more at
  [shields.io](https://shields.io) / [simpleicons.org](https://simpleicons.org).
- **Accent color** — I used purple (`A855F7`) throughout. Find/replace it with any hex to re-theme.

That's it. Commit, refresh your profile, done. 💜
