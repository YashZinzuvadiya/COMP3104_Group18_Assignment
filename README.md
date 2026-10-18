# COMP3104_Group18_Assignment

## Group Members
- **Leader:** Yash Zinzuvadiya (101475983) - [GitHub](https://github.com/YashZinzuvadiya)
- **Member 2:** Yatin Korat (101560107) - [GitHub](https://github.com/yatinkorat)
- **Member 3:** Ishan Sood (101539944) - [GitHub](https://github.com/Ishannsood)
- **Member 4:** Rabin Kunnananickal Binu (101516420) - [GitHub](https://github.com/rabinkbinu)

## Project Description
This repository hosts the Group 18 assignment for the DevOps course. It practises collaborative Git workflows: per-developer branches, regular commits, pull requests, merge conflict resolution, a pull request template and continuous integration with GitHub Actions. Each member contributes three text files covering George Brown College, the DevOps course and the role of DevOps in the software development lifecycle.

## Setup Instructions
1. Clone the repository: `git clone https://github.com/YashZinzuvadiya/COMP3104_Group18_Assignment.git`
2. Enter the folder: `cd COMP3104_Group18_Assignment`
3. Create your own branch: `git checkout -b STUDENTID-Name`
4. Push it: `git push -u origin STUDENTID-Name`
5. Commit locally, run `git pull origin main` regularly, and open a pull request into `main` when ready.

## CI/CD Pipeline
GitHub Actions runs the workflow in `.github/workflows/ci.yml` on every push and on pull requests to `main`. It runs on `ubuntu-latest`, checks out the code, lists the repository files and confirms that `README.md` exists. The status of each run is shown in the Actions tab.

## Branching Strategy
The team uses a per-developer branching strategy. Each member works on a personal branch named `STUDENTID-Name` (for example `101475983-Yash`). Nobody commits directly to `main`. Changes reach `main` through pull requests that use the pull request template, and any merge conflicts are resolved before merging.
