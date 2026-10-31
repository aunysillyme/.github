# .github

Account-wide defaults for aunysillyme repos: funding links, contributing guide, SECURITY.md, support page and issue forms. A repository's own file of the same type replaces the default.

## Set sync

Changes to `set.json` or `set-sync.targets.json` on `main` start a workflow that updates the shared set data and generated set blocks in each target repository. When files change, it opens or updates a pull request and enables squash auto-merge. To run it by hand, open Actions, select **Set sync**, and choose **Run workflow** on `main`.
