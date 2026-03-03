# Stash

Local-first, conflict-free file sync using Automerge CRDTs. Repo: `~/Repos/stash`

## Bugs

- `stash create` crashes on empty GitHub repos (tries to fetch ref that doesn't exist)
- `stash create` shows interactive prompt when stdin is not a TTY — needs a `--yes` flag or auto-detect
- `status` shows 0 files after `create`/`connect` when `.git` is present in the directory. Removing `.git` fixes it. Likely the chokidar `ignored` pattern `/[/\\]\./` is too broad (matches any path component starting with `.`), or `initializeSnapshots` is affected. The `connect` path also never renders CRDT docs to disk.
- GitHub API rate limit: "Request quota exhausted for POST /repos/{owner}/{repo}/git/blobs" — need to handle rate limiting gracefully, and possibly batch blob creation or reduce API calls during sync
- `stash delete` has no `--yes` flag either (same interactive prompt issue as create)

## Next steps

- Fix the above bugs (blocking agent sync setup)
- Review test coverage around create-with-existing-dir, connect, and reconciler flush
- Get ready for release
