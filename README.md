# COMP3104_Group18_Assignment


## Branching Details

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


## CI/CD Pipeline

Our pipeline is a GitHub Actions workflow in `.github/workflows/ci.yml`. It is named **CI**, and each run shows who triggered it and on which branch.

### Triggers
- **push:** runs on every push to any branch.
- **pull_request:** runs when a pull request is opened or updated against `main`.

### Runner
One job called `build` runs on a GitHub-hosted `ubuntu-latest` machine.

### Steps
1. **Check out repository code:** uses `actions/checkout@v4` to download the repo.
2. **Print the trigger:** prints which event started the run and the runner's OS.
3. **List repository files:** runs `ls -la` to show the files in the repo.
4. **Check required files exist:** runs `test -f README.md`. If the README is missing, the step fails and the run turns red.

A green check on a branch means all steps passed.

## Group Members
- **Leader:** Yash Zinzuvadiya (101475983) - [GitHub](https://github.com/YashZinzuvadiya)
- **Member 2:** Yatin Korat (101560107) - [GitHub](https://github.com/yatinkorat)
- **Member 3:** Ishan Sood (101539944) - [GitHub](https://github.com/Ishannsood)
- **Member 4:** Rabin Kunnananickal Binu (101516420) - [GitHub](https://github.com/rabinkbinu)

## Project Description
This is our Group 18 assignment for the COMP3104 DevOps course. We practise working as a team on GitHub. Each member has their own branch, makes regular commits and merges through a pull request. The repository also has a GitHub Actions workflow that runs on every push. Each member added three text files about George Brown College, the DevOps course and DevOps in the software development life cycle.

## Setup Instructions
1. Accept the invitation to the repository on GitHub.
2. Clone the repository and open the folder:
   `git clone https://github.com/YashZinzuvadiya/COMP3104_Group18_Assignment.git`
   `cd COMP3104_Group18_Assignment`
3. Make your own branch named with your student ID and name, for
   example `101560107-Yatin`, and push it:
   `git checkout -b 101560107-Yatin`
   `git push -u origin 101560107-Yatin`
4. Create your three text files in the main folder, then commit and
   push your work regularly from your own computer.
5. Run `git pull origin main` before each work session to stay up to
   date, and open a pull request into `main` when you are done.

## CI/CD Pipeline
GitHub Actions runs the workflow in `.github/workflows/ci.yml` on every push and on pull requests to `main`. It runs on `ubuntu-latest`, checks out the code, lists the repository files and confirms that `README.md` exists. The status of each run is shown in the Actions tab.

## Branching Strategy
The team uses a per-developer branching strategy. Each member works on a personal branch named `STUDENTID-Name` (for example `101475983-Yash`). Nobody commits directly to `main`. Changes reach `main` through pull requests that use the pull request template, and any merge conflicts are resolved before merging.

