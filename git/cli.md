# Git

## Settings

- Add your *username*:

  ```sh
  $ git config --global user.name "<username>"
  ```

- Add your *email*:

  ```sh
  $ git config --global user.email "<email>"
  ```

- Check if everything is alright:

  ```sh
  $ git config --list
  ```

*This may seem trivial, but actually it's really important. If your credentials
are not properly set, your commits will not appear as yours.*

- If you want to clean your *username* and *email* just type:

  ```sh
  $ git config --global --unset-all user.name && git config --global --unset-all user.email
  ```

## Repositories

- Create a new repository:

  ```sh
  $ git init
  ```

## Clone

- Clone a repository:

  ```sh
  $ git clone <repository>
  ```

  *Clone a repository directly into the current directory (if empty):*

  ```sh
  $ git clone <repository> .
  ```

## Commits

- Check for changes:

  ```sh
  $ git status
  ```

- Stage all changes to be committed:

  ```sh
  $ git add -A
  ```

- Commit your changes:

  ```sh
  $ git commit -m <message>
  ```

## Branches

- List all branches:

  ```sh
  $ git branch
  ```

- Create a branch:

  ```sh
  $ git branch <branch-name>
  ```

  *Create a branch and automatically switch to it:*

  ```sh
  $ git checkout -b <branch-name>
  ```

- Switch to another branch:

  ```sh
  $ git checkout <branch-name>
  ```

- Delete a branch:

  ```sh
  $ git branch -d <branch-name>
  ```

## Remotes

- Add a remote:

  ```sh
  $ git remote add <remote-name> <repository>
  ```

- Pull changes from remote repository:

  ```sh
  $ git pull <remote-name> <branch-name>
  ```

## Stash

- Stash changes:

  ```sh
  $ git stash
  ```

  *Stash changes with a descriptive message:*

  ```sh
  $ git stash save <message>
  ```

  *Stash changes —including untracked files— with a descriptive message:*

  ```sh
  $ git stash save -u <message>
  ```

- List stash entries:

  ```sh
  $ git stash list
  ```

- Apply saved changes from the latest stash entry:

  ```sh
  $ git stash pop
  ```

  *Apply saved changes from the indicated stash entry:*

  ```sh
  $ git stash pop 'stash@{n}'
  ```

- Remove all stash entries:

  ```sh
  $ git stash clear
  ```

## Rebase

- Squash commits with (interactive) rebase:

  ```sh
  $ git rebase -i <branch>
  ```

  *In case of conflict, solve them and then continue with the rebase:*

  ```sh
  $ git rebase --continue
  ```

- Abort rebase:

  ```sh
  $ git rebase --abort
  ```

## Others

### Rename case-sensitive file

- Rename a file to the same name but with a different case:

  ```sh
  $ git mv FILE FILE.tmp && git mv FILE.tmp file
  ```
