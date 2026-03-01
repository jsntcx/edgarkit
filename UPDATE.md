# When the upstream fixes it or you want other updates

1. Add upstream as a remote in your fork: git remote add upstream <https://github.com/r007/edgarkit>
2. git fetch upstream && git merge upstream/master
3. Resolve any conflict on that one field (trivial since it's one attribute line)
4. Push — your workspace picks it up on next cargo update

This keeps your patch minimal and isolated to one commit, making merges trivial forever.
