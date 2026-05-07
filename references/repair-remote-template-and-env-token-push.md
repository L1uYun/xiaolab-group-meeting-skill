# repair remote template and env token push

## Scope
When the public xiaolab template is synced but still low-quality, separate two tracks:
1. sync status
2. template quality status

## Durable repair order
1. Fix the public checkout template first.
2. Mirror the same file into the Hermes loaded skill path.
3. Preview locally.
4. Source `~/.hermes/.env` if the current shell cannot see GitHub token vars.
5. Push with one-shot token URL.
6. `git fetch` and verify `HEAD == origin/main`.

## Concrete token rule
Current shell missing `GITHUB_TOKEN` does not prove the machine lacks credentials.
Check:
- `GITHUB_TOKEN`
- `GH_TOKEN`
- `GITHUB_PAT`
- `~/.hermes/.env`

If needed:
```bash
set -a
source ~/.hermes/.env
set +a
```

Then push once via:
```bash
https://x-access-token:${GITHUB_TOKEN}@github.com/owner/repo.git
```

## Template-quality lesson
For xiaolab borrowing from guizang:
- borrow deck engine, theme switching, dots, overview, fullscreen, and lightweight animation
- do not copy keynote rhetoric or magazine interstitials
- keep xiaolab as group-meeting deck, not external-talk deck
