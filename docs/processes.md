# ⚙️ Processes & Conventions

Shared conventions so everyone works the same way.

## Git workflow

We use a simple **branch → Pull Request → review → merge** flow. Never commit
directly to `main` / `master`.

1. **Create a branch** from the default branch:
   ```bash
   git checkout -b <type>/<short-description>
   # e.g. feat/sponsor-section, fix/navbar-mobile
   ```
2. **Commit** in small, focused steps (see commit conventions below).
3. **Push** and open a **Pull Request**.
4. Request a **review** from a teammate (HoD/ToD or a division member).
5. Address feedback, then **merge** (squash is fine for small PRs).

### Branch naming

| Prefix | When to use |
|--------|-------------|
| `feat/` | New feature |
| `fix/` | Bug fix |
| `docs/` | Documentation only |
| `refactor/` | Code change without behavior change |
| `chore/` | Tooling, config, maintenance |

### Commit messages

Keep them short and in the imperative mood. Optionally use a prefix matching
the branch type:

```
feat: add sponsor carousel to home page
fix: hamburger menu not opening on mobile
docs: document deploy workflow
```

### Pull Requests

- Give it a clear title and a short description of **what** and **why**.
- Keep PRs small and focused — easier to review.
- Make sure the project **builds** before requesting review.
- At least **one approval** before merging (when possible).

## Code & asset conventions

- **Asset filenames are case-sensitive** on the production server (Linux).
  Reference files in code with the **exact** name (including capitals),
  otherwise images break in production but work locally on Windows/macOS.
- Keep secrets out of the repo — use environment variables / GitHub Secrets.
- Prefer reusing existing components and utilities over duplicating code.

## Meetings

- **Regular team/division meetings** — keep short notes and action items.
- Share recurring info (dates, links) in the team chat and, if long-lived,
  add it to this handbook.

## Document management

- **Code & technical docs** → GitHub (this handbook, repo READMEs, `docs/`).
- **Design files, large media, datasheets** → shared Google Drive.
- **Public-facing info** → the [website](https://politocean.polito.it).

> 🤝 This handbook is open to contributions. See a gap or an error? Open a PR.
