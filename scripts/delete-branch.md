# Branch Deletion Guide

To delete a branch via the GitHub API, use:

```bash
curl -X DELETE -H "Authorization: token YOUR_TOKEN" \
  https://api.github.com/repos/OWNER/REPO/git/refs/heads/BRANCH_NAME
```

This works by deleting the git reference that points to the branch, effectively removing the branch from the repository.
