# .github

Account-wide defaults for aunysillyme repos: funding links, contributing guide, SECURITY.md, support page and issue forms. A repository's own file of the same type replaces the default.

## Set sync

Changes to `set.json` or `set-sync.targets.json` on `main` start the workflow. Set repositories must already have their sync inputs; the workflow runs set sync and updates their generated blocks. Extra targets receive only a byte-identical `.repo-build/set.json`. When files change, it opens or updates a pull request and attempts to enable squash auto-merge. When no files change, it closes stale sync pull requests and deletes their branch. Preparation and publishing use separate runners so target scripts cannot change the Git configuration or hooks used with the app token. To run it by hand, open Actions, select **Set sync**, and choose **Run workflow** on `main`.
