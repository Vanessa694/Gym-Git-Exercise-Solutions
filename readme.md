# git exercises 

## bundle 1

### exercise 1

'''bash
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git init
Reinitialized existing Git repository in /Users/gymuruhimbiii/bundle1/exercise1/exercise1.1/.git/
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -M bundle1
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git statusd
git: 'statusd' is not a git command. See 'git --help'.

The most similar command is
        status
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch bundle1

No commits yet

nothing to commit (create/copy files and use "git add" to track)
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch bundle1

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git add readme.md
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status 
On branch bundle1

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md

gymuruhimbiii@uruhimbis-iMac exercise1.1 % git commit -m "init exercise"
[bundle1 (root-commit) 81c0913] init exercise
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git remote add origin https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch bundle1
nothing to commit, working tree clean
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
fatal: The current branch bundle1 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin bundle1

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push --set-upstream origin bundle1
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 234 bytes | 234.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
 * [new branch]      bundle1 -> bundle1
branch 'bundle1' set up to track 'origin/bundle1'.
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
Everything up-to-date
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git checkout -b dev
Switched to a new branch 'dev'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch dev
nothing to commit, working tree clean
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push 
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Vanessa694/Gym-Git-Exercise-Solutions/pull/new/dev
remote: 
To https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -m <bundle1> <main>
zsh: parse error near `<'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch dev
nothing to commit, working tree clean
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push --set-upstream origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -M main           
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push --set-upstream origin main   
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
^[[A^[[Aremote: 
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/Vanessa694/Gym-Git-Exercise-Solutions/pull/new/main
remote: 
To https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
^[[A%                                                                                             
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push                              
Everything up-to-date
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -d <bundle1>
zsh: parse error near `\n'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
Everything up-to-date
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git checkout <main> 
zsh: parse error near `\n'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -d <bundle1>
zsh: parse error near `\n'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
Everything up-to-date
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -d bundle1
Deleted branch bundle1 (was 81c0913).
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
Everything up-to-date
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push origin --delete bundle1
To https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
 ! [remote rejected] bundle1 (refusing to delete the current branch: refs/heads/bundle1)
error: failed to push some refs to 'https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch
* main
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -a
* main
  remotes/origin/bundle1
  remotes/origin/dev
  remotes/origin/main
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -M main
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -D bundel1
error: branch 'bundel1' not found.
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push origin --delete bundle1
To https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
 ! [remote rejected] bundle1 (refusing to delete the current branch: refs/heads/bundle1)
error: failed to push some refs to 'https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -D bundle1
error: branch 'bundle1' not found.
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git checkout -b dev                
Switched to a new branch 'dev'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git status 
On branch dev
nothing to commit, working tree clean
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push origin dev               
Everything up-to-date
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git checkout -b test
Switched to a new branch 'test'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Vanessa694/Gym-Git-Exercise-Solutions/pull/new/test
remote: 
To https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git checkout dev    
Switched to branch 'dev'
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git branch -d test
Deleted branch test (was 81c0913).
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push origin --delete test
To https://github.com/Vanessa694/Gym-Git-Exercise-Solutions.git
 - [deleted]         test
gymuruhimbiii@uruhimbis-iMac exercise1.1 % git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymuruhimbiii@uruhimbis-iMac exercise1.1 % 
'''bash