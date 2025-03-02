# template

# GitHub Actions
This repository comes with 2 (actually 3) GitHub Actions:

. scaffolder: it removes itself after the first run, so you won't see it, but it is used to replace placeholder values like <<< SCAFFOLDER_REPO_NAME >>> from the template repo
. updater: runs every month to fetch updates from the template and opens a PR with suggested changes - be aware that it will always favor the template in case of merge conflicts, so you definetely need to review the changes and adapt it accordingly
. <<< SCAFFOLDER_REPO_NAME >>>: the actual CI/CD pipeline of this repository, taken care of build, scans, staging, testing and production deployment
