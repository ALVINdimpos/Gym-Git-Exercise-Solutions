## BUNDLE 1
# Exercise 1
```
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % echo "# Git-Exercises" >> README.md
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git init 
Initialized empty Git repository in /Users/andelarwanda/Desktop/Gym Git Exercise Solutions/.git/
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git add .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git commit -m "Initial comit"
[master (root-commit) 95fe4e2] Initial comit
 Committer: ALVIN CODER <andelarwanda@Andelas-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 README.md
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git remote add https://github.com/ALVINdimpos/Git-Exercises.git
usage: git remote add [<options>] <name> <url>

    -f, --fetch           fetch the remote branches
    --tags                import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --track <branch>  branch(es) to track
    -m, --master <branch>
                          master branch
    --mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git remote add origin https://github.com/ALVINdimpos/Git-Exercises.git
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch --m master main
error: ambiguous option: m (could be --move or --merged)
usage: git branch [<options>] [-r | -a] [--merged | --no-merged]
   or: git branch [<options>] [-l] [-f] <branch-name> [<start-point>]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track           set up tracking mode (see git-pull(1))
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      Unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display SHA-1s

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch debv
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch -d debv
Deleted branch debv (was 95fe4e2).
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch dev
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git checkout dev
Switched to branch 'dev'
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git checkout dev
Already on 'dev'
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch
* dev
  main
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch test
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch
* dev
  main
  test
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch -d test
Deleted branch test (was 95fe4e2).
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch
* dev
  main
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git add .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git commit -m 'Added readme' 
[dev 823d156] Added readme
 Committer: ALVIN CODER <andelarwanda@Andelas-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git push origin dev 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 283 bytes | 283.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/ALVINdimpos/Git-Exercises/pull/new/dev
remote: 
To https://github.com/ALVINdimpos/Git-Exercises.git
 * [new branch]      dev -> dev
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % 
```
