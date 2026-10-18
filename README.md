# COMP3104_Group18_Assignment

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