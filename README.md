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
# Exercise 1
```
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % $ git stash save "Save changes for home page"

zsh: command not found: $
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git add .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash
Saved working directory and index state WIP on dev: 823d156 Added readme
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git add .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash
Saved working directory and index state WIP on dev: 823d156 Added readme
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git add .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash
Saved working directory and index state WIP on dev: 823d156 Added readme
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git status
On branch dev
nothing to commit, working tree clean
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash pop about.html
error: about.html is not a valid reference
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash pop 1         
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped refs/stash@{1} (3482ab5afc52b8852dc1d17bc98a48fd319caa9e)
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git commit -m "ave changes for about page"
[dev 02c72a0] ave changes for about page
 Committer: ALVIN CODER <andelarwanda@Andelas-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 24 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 498 bytes | 498.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/ALVINdimpos/Git-Exercises.git
   823d156..02c72a0  dev -> dev
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash pop 2
fatal: Log for 'refs/stash' only has 2 entries.
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash pop 1
On branch dev
nothing to commit, working tree clean
Dropped refs/stash@{1} (27b65dca2cd5169e30cbcb4d7bc4d6c4b77a1887)
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (eef21e0b48d6bb4b9c2a1ee39ea8ba31413e6cae)
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git reset HEAD .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git reset
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git reset --hard
HEAD is now at 02c72a0 ave changes for about page
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git reset --soft
```
## BUNDLE 2
# Exercise 1
```
git bransh ft/bundle-2
git: 'bransh' is not a git command. See 'git --help'.

The most similar command is
        branch
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git branch ft/bundle-2
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git add .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git add .
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git commit -m 'Added service.html page'
[ft/bundle-2 bbdfd20] Added service.html page
 Committer: ALVIN CODER <andelarwanda@Andelas-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 12 insertions(+)
 create mode 100644 services.html
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % git push origin ft/bundle-2
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 273 bytes | 273.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/ALVINdimpos/Git-Exercises/pull/new/ft/bundle-2
remote: 
To https://github.com/ALVINdimpos/Git-Exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
andelarwanda@Andelas-MacBook-Pro Gym Git Exercise Solutions % 
```
# Exercise 2
```
 Gym Git Exercise Solutions git:(ft/bundle-2) git checkout main           
Switched to branch 'main'
➜  Gym Git Exercise Solutions git:(main) git pull origin main
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From https://github.com/ALVINdimpos/Git-Exercises
 * branch            main       -> FETCH_HEAD
   95fe4e2..3484c50  main       -> origin/main
Updating 95fe4e2..3484c50
Fast-forward
 README.md     |  1 +
 about.html    | 12 ++++++++++++
 home.html     | 12 ++++++++++++
 services.html | 12 ++++++++++++
 4 files changed, 37 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
➜  Gym Git Exercise Solutions git:(main) git checkout -b ft/service-redesign    
Switched to a new branch 'ft/service-redesign'
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git add .                          
➜  Gym Git Exercise Solutions git:(ft/service-redesign) ✗ git commit -m "ft/services-redesign: added servecs page"
[ft/service-redesign e22a201] ft/services-redesign: added servecs page
 Committer: ALVIN CODER <andelarwanda@Andelas-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 7 insertions(+)
 rename services.html => service.html (59%)
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git push oriigin ft/services-redesigm
error: src refspec ft/services-redesigm does not match any
error: failed to push some refs to 'oriigin'
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git push origin ft/services-redesign 
error: src refspec ft/services-redesign does not match any
error: failed to push some refs to 'https://github.com/ALVINdimpos/Git-Exercises.git'
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git push origin ft/services-redesign -f
error: src refspec ft/services-redesign does not match any
error: failed to push some refs to 'https://github.com/ALVINdimpos/Git-Exercises.git'
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git push -f                            
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

➜  Gym Git Exercise Solutions git:(ft/service-redesign) git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 536 bytes | 536.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/ALVINdimpos/Git-Exercises/pull/new/ft/service-redesign
remote: 
To https://github.com/ALVINdimpos/Git-Exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
Branch 'ft/service-redesign' set up to track remote branch 'ft/service-redesign' from 'origin'.
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git giff                                          
git: 'giff' is not a git command. See 'git --help'.

The most similar command is
        diff
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git diff

➜  Gym Git Exercise Solutions git:(ft/service-redesign) git merge main
Already up to date.
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git checout main                                        
git: 'checout' is not a git command. See 'git --help'.

The most similar command is
        checkout
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git checkout main                  
Switched to branch 'main'
➜  Gym Git Exercise Solutions git:(main) git add .        
➜  Gym Git Exercise Solutions git:(main) ✗ git commit -m "Added some  changes"                      
[main fd573f1] Added some  changes
 Committer: ALVIN CODER <andelarwanda@Andelas-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 7 insertions(+)
 rename services.html => service.html (59%)
➜  Gym Git Exercise Solutions git:(main) git push                                          
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

➜  Gym Git Exercise Solutions git:(main) git push --set-upstream origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 525 bytes | 525.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/ALVINdimpos/Git-Exercises.git
   3484c50..fd573f1  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
➜  Gym Git Exercise Solutions git:(main) git checkout ft/services-redesign  
error: pathspec 'ft/services-redesign' did not match any file(s) known to git
➜  Gym Git Exercise Solutions git:(main) git pull                           
Already up to date.
➜  Gym Git Exercise Solutions git:(ft/service-redesign) git merge main           
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
➜  Gym Git Exercise Solutions git:(ft/service-redesign) ✗ git add       
Nothing specified, nothing added.
Maybe you wanted to say 'git add .'?
➜  Gym Git Exercise Solutions git:(ft/service-redesign) ✗ git  merge --continue
U       service.html
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
➜  Gym Git Exercise Solutions git:(ft/service-redesign) ✗ git  merge --continue
U       service.html
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
➜  Gym Git Exercise Solutions git:(ft/service-redesign) ✗ git commit -m "feat: solved a conflict"
U       service.html
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
➜  Gym Git Exercise Solutions git:(ft/service-redesign) ✗ git add .                              
➜  Gym Git Exercise Solutions git:(ft/service-redesign) ✗ git commit -m "feat: solved a conflict"
[ft/service-redesign 5eea256] feat: solved a conflict
 Committer: ALVIN CODER <andelarwanda@Andelas-MacBook-Pro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

➜  Gym Git Exercise Solutions git:(ft/service-redesign) git push -f                            
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 353.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ALVINdimpos/Git-Exercises.git
   e22a201..5eea256  ft/service-redesign -> ft/service-redesign
➜  Gym Git Exercise Solutions git:(ft/service-redesign) 
```
