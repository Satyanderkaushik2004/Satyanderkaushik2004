# Setup

This repo powers your GitHub profile README — the special repo named exactly the
same as your username (e.g. `Satyanderkaushik2004/Satyanderkaushik2004`).

1. **Create the profile repository**, if you don't have it yet: on GitHub, create a
   new **public** repo named exactly your username. GitHub auto-detects it and
   shows its README on your profile page.
2. **Replace the files** in that repo with everything in this folder
   (`README.md`, `assets/`, `.github/`, this file, `ASSET-MAP.md`, `config.md`).
3. **Update your info** — open `config.md`, then find-and-replace those values
   throughout `README.md` (see "What to edit" below).
4. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Rebuild profile README"
   git push origin main
   ```
5. **Enable GitHub Actions** — go to the repo's **Actions** tab and enable
   workflows if prompted. This runs `.github/workflows/snake.yml`.
6. **Wait for the snake to generate** — the workflow runs automatically on push
   and once a day after that. You can also trigger it manually from the
   **Actions** tab (**Run workflow**). It publishes SVGs to a branch called
   `output`, which the README already points to.
7. **Open your profile** — `https://github.com/<your-username>` — and check
   that the hero image, stats cards, and snake animation are all rendering.

---

## What to edit

Everything below currently points at the placeholder handle
`Satyanderkaushik2004`. Replace it with your actual GitHub username everywhere
it appears in `README.md`:

- Every `github-readme-stats.vercel.app`, `github-readme-streak-stats`, and
  `github-profile-trophy` URL (`?username=...`)
- The `github.com/<username>.png` avatar URL
- The snake `<picture>` / `<img>` source URLs
- All GitHub profile links

Also update, in `README.md`:

| Field | Where |
|---|---|
| Email | "Let's Connect" section + sidebar |
| LinkedIn URL | sidebar + "Let's Connect" |
| Portfolio URL | sidebar + "Let's Connect" (currently `vyomedu.in`) |
| Project repo links | "Featured Projects" (`KAIROS` and `BitVault` are placeholders) |
| Location | sidebar |

`config.md` lists all of these values in one place for quick reference.

---

## Notes

- The snake workflow needs **Actions write permission** for `GITHUB_TOKEN`.
  If the push step fails with a permissions error, go to **Settings → Actions
  → General → Workflow permissions** and set it to **Read and write
  permissions**.
- GitHub stats/streak/trophy cards are rendered live by third-party services
  (`github-readme-stats`, `github-readme-streak-stats`,
  `github-profile-trophy`) — nothing is hard-coded, so they'll show your real
  numbers automatically once the username is correct.
- If a stats card doesn't load, it's usually that free service being briefly
  rate-limited — reload after a minute, or self-host the service if it
  persists (instructions in each project's own repo).
