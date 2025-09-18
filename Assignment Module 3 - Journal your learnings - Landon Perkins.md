# Journal — Chapters 8 & 9: GitHub Primer / Quick Start
# Key takeaways
-   **What GitHub is:** not just code hosting it's a development platform for hosting/reviewing code, managing projects, and publishing sites/apps.
-   **Core open-source flow:** Fork → edit your copy → open a Pull Request → review → merge (or discuss).
-   **Docs hierarchy:** `README.md` (quick intro + install + how to contribute), **Wiki** (longer guides; its own git repo), **GitHub Pages** (host a site from a repo).
-   **Roles beyond code:** docs writers, translators, community managers, testers — all matter.
-   **Personal perks:** private repos, portfolio via Pages, stars/followers, contribution graph.
-   **Business:** paid/enterprise features exist, but Free works for learning.
-   **Remote vs local:** `git init` = local repo; create a remote repo on GitHub and connect with `git remote add <name> <url>` (usually `origin`). `git push` publishes; `git pull` fetches.
-   **Basics to remember:** `git init` / `git clone <url>`; `git add` → `git commit`; `git remote -v`; `git push origin <branch>` (branch may be `main` or `master`).
# Difficulties / things to watch
-   **Auth friction:** old creds or password managers block pushes — set up SSH keys or a personal access token (PAT).
-   **Branch name:** default may be `main` or `master` — always check before pushing.
-   **Fork vs clone:** _Fork_ = copy on your account for PRs; _Clone_ = local copy (of fork or original).
-   **Docs choice:** `README` for quick start; Wiki for long docs; Pages for a public site.
-   **Visibility & limits:** public = anyone can read; private = limited collaborators (check current plan).
-   **Push semantics:** `git push` updates a branch; if histories diverge you’ll need to pull/rebase or resolve conflicts.
# Quick reference & troubleshooting
-   Link remote: `git remote add origin https://github.com/<username>/<repo>.git`
-   Push initial commit: ``git add README.md`` and ``git commit -m "Initial commit" git push origin master or `main` `` 
-   Check remotes: `git remote -v`
-   Remove remote: `git remote rm <name>`
-   Force credential re-prompt: `git config --local credential.helper ""`
-   Switch to SSH if auth fails: `git remote set-url origin git@github.com:<user>/<repo>.git`
-   If push rejected due to diverging history: `git pull --rebase` or fetch, merge, then push.
# Reflection / next steps
-   Chapter does a good job moving from concept → practice.
-   Focus next on branching, merge conflicts, and PR workflow — those are the most useful next steps.