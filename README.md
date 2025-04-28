pwd
mkdir mashashadow

cd mashashadow/


$ git init
Initialized empty Git repository in C:/Users/IS/mashashadow/.git/


$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)


$ git remote add https://github.com/mas-marmar/dosochka.git
usage: git remote add [<options>] <name> <url>

    -f, --[no-]fetch      fetch the remote branches
    --[no-]tags           import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --[no-]track <branch>
                          branch(es) to track
    -m, --[no-]master <branch>
                          master branch
    --[no-]mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from


is@MK-201-004 MINGW64 ~/mashashadow (master)
$ git remote -v

is@MK-201-004 MINGW64 ~/mashashadow (master)
$ git remote add  https://github.com/mas-marmar/dosochka.git
usage: git remote add [<options>] <name> <url>

    -f, --[no-]fetch      fetch the remote branches
    --[no-]tags           import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --[no-]track <branch>
                          branch(es) to track
    -m, --[no-]master <branch>
                          master branch
    --[no-]mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from

$ git remote -v

$ git remote add origin ^[[200~git@github.com:mas-marmar/dosochka.git~

$ git remote add origin git@github.com:mas-marmar/dosochka.git
error: remote origin already exists.

$ git remote -v
origin  git@github.com:mas-marmar/dosochka.git~ (fetch)
origin  git@github.com:mas-marmar/dosochka.git~ (push)

$ touch README.md

$ explorer .

$ git add .

$ git commit -m "dh"
[master (root-commit) 7e22991] dh
 Committer: Студент группы IS <is@sielom.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 1 insertion(+)
 create mode 100644 README.md
 create mode 100644 meow.txt

$  git config --global user.name "da"

$  git config --global user.email "masamaslakova@gmail.com"

$ git commit -m "dh"
On branch master
nothing to commit, working tree clean

$ git status
On branch master
nothing to commit, working tree clean

$ git push -u origin master
\033[200~git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

$ git push -u origin master
\033[200~git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

$ git remote -v
origin  git@github.com:mas-marmar/dosochka.git~ (fetch)
origin  git@github.com:mas-marmar/dosochka.git~ (push)

$ git remote remove origin

$ git remote -v

$ git remote add origin https://github.com/mas-marmar/dosochka.git

$ git push -u origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 295 bytes | 295.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/mas-marmar/dosochka.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
