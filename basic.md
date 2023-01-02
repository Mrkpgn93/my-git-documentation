# Basics :abc:

1. [Working tree status :herb:](#working-tree-status)
1. [Is there any repo? :open_file_folder:](#is-there-any-repo)
1. [Add file to the index :clipboard:](#add-file-to-the-index)
1. [Fix the state of a repo :ring:](#fix-the-state-of-a-repo)
1. [Logs :notebook_with_decorative_cover: :anchor:](#logs)
1. [How to modify last commit :wrench:](#logs)
1. [Add and commit at once :clipboard::ring:](#add-and-commit-at-once)

## Working tree status

`git status` [:link:](https://git-scm.com/docs/git-status)

> Displays paths that have differences between the index file and the current HEAD commit, paths that have differences between the working tree and the index file, and paths in the working tree that are not tracked by Git

---

## Is there any repo?

`git init` [:link:](https://git-scm.com/docs/git-init)

> Create an empty Git repository or reinitialize an existing one

---

## Add file to the index

`git add <file-name> <file-name2>...` [:link:](https://git-scm.com/docs/git-add#Documentation/git-add.txt-ltpathspecgt82308203)

`git add .` [:link:](https://git-scm.com/docs/git-add)

`git add --all` [:link:](https://git-scm.com/docs/git-add#Documentation/git-add.txt---all)

> This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit. It typically adds the current content of existing paths as a whole, but with some options it can also be used to add content with only part of the changes made to the working tree files applied, or remove paths that do not exist in the working tree anymore.

---

## Fix the repo's state

`git commit -m "msg"` [:link:](https://git-scm.com/docs/git-commit)

> Create a new commit containing the current contents of the index and the given log message describing the changes.

---

## Logs

`git log` [:link:](https://git-scm.com/docs/git-log)

`git log --oneline` [:link:](https://git-scm.com/docs/git-log#Documentation/git-log.txt---oneline)

`git log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all
` [:link:](https://git-scm.com/docs/git-log#Documentation/git-log.txt---graph)

> List commits that are reachable by following the parent links from the given commit(s), but exclude commits that are reachable from the one(s) given with a ^ in front of them. The output is given in reverse chronological order by default.

---

## How to modify last commit

`git commit --amend` [:link:](https://git-scm.com/docs/git-commit#Documentation/git-commit.txt---amend)

> I can only go back one step! it comes in handy when I have to change the commit message or add something I forgot inside the stage (in the latter case I have to precede the amend command from the add one)

---

## Add and commit at once

`git commit -a -m "msg"`

> It's the equivalent of _"git add ." + "git commit"_
