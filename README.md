# COMP3104_Group18_Assignment
## Group Members
- Rabin Kunnananickal Binu (101516420) – [rabinkbinu](https://github.com/rabinkbinu)

## Branching Strategy

We use a feature-branch workflow. Each member works on their own branch, and changes reach `main` only through pull requests.

| Branch | Owner | Purpose |
|---|---|---|
| `main` | Group | Stable branch, updated only by merging PRs |
| `101475983-Yash` | Yash | CI workflow, PR template, individual files |
| `101560107-Yatin` | Yatin | README top section, individual files |
| `101539944-Ishan` | Ishan | CI/CD section, individual files |
| `101516420-Rabin` | Rabin | Branching and conflict notes, individual files |

**Workflow**
1. Run `git pull origin main` before each work session.
2. Make small commits with clear messages and push regularly.
3. Before opening a PR, merge the latest `main` into your branch and resolve conflicts locally.
4. Open a PR into `main` using the PR template and confirm CI passes.
5. Merge with **Create a merge commit** (no squash) and keep the branch.

**Merge order:** Yash → Yatin → Ishan → Rabin, one PR at a time.