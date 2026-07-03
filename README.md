# cross-functional-lab
"Merge vs Rebase" — the presentation topic, answered:

Merge: combines two branches by creating a new merge commit. Preserves complete, non-destructive history — you can see exactly when and how branches diverged and rejoined. Can create a "messier" history with lots of merge commits.
Rebase: replays your branch's commits on top of the target branch, producing a clean, linear history. Rewrites commit hashes — never rebase a branch others are already working on, since it breaks shared history. Rebase is generally preferred for keeping a clean commit history on local feature branches before sharing them with others.
Rule of thumb: rebase local/private branches to keep history clean before pushing; merge when integrating into shared/protected branches like main.
