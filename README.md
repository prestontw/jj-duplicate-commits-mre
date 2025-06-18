## Duplicate commits in GitHub's PR view using JJ

I've been playing around with using `jj` at work, and generally really enjoying it.
However, there were two cases when I noticed duplicate commits for my work in the PR I submitted to GitHub.
By "duplicate commits," I mean work that was in `main` that showed up in my branch after merging `main` into my work.
Usually, using `git`, I'll just `git merge main`, `git push`, and my branch will be up to date and the commits since I initially cut my branch won't show up in the PR in GitHub.
However, using `jj new @ main`, I ended up with commits from `main` that I didn't author and that wouldn't be there in the `git` case showing up in my PR, making my PR harder to review.
Concerned, I tried to recreate this but could not.
I ran into this again later after merging `main` in twice to a `jj` stream.

This repo is me trying to recreate the conditions for when commits from `main` show up in my PR's.
