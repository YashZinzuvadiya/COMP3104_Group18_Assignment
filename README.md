# COMP3104_Group18_Assignment

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