This repo demonstrates [Viewing missing commit details from commits in your timeline](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/managing-contribution-settings-on-your-profile/troubleshooting-commits-on-your-timeline#viewing-missing-commit-details-from-commits-in-your-timeline) in GitHub Docs.

## How it works?

See [Git Docs](https://git-scm.com/docs/git-commit#_commit_information)

```cmd
set "GIT_AUTHOR_NAME=octocat"
set "GIT_AUTHOR_EMAIL=octocat@nowhere.com"
set "GIT_AUTHOR_DATE=Tue, 03 Apr 2018 02:02:30 +0900"
set "GIT_COMMITTER_NAME=Sally Johnson"
set "GIT_COMMITTER_EMAIL=USER_EMAIL"
set "GIT_COMMITTER_DATE=Tue, 10 Apr 2018 06:25:08 +0900"
git commit -m init --reset-author
git tag YOUR_COMMIT_SHA_NUMBER HEAD
git show YOUR_COMMIT_SHA_NUMBER --pretty=fuller
```
