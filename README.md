# Git Branching & Merge-Conflict Demo

Small sample project used to demonstrate a real Git branching workflow
and a real merge conflict + resolution, for the Complex Engineering
Problem report on "Git Branching Strategy and Merge Conflict Resolution".

## Branches
- `main` – stable branch
- `develop` – integration branch
- `feature/login` – adds a login attempt limit
- `feature/payment` – adds a payment timeout (and also touches the same line)

## What happened here
1. Two feature branches were created from `develop`.
2. Both branches edited the same line in `config.js`.
3. `feature/login` merged into `develop` cleanly.
4. `feature/payment` merge into `develop` produced a real merge conflict.
5. The conflict was resolved by hand, keeping both intended changes.
6. A GitHub Actions workflow runs a basic check on every push/PR.

Run `git log --all --graph --oneline` after cloning to see the full history.
