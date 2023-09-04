# Git Pratice Documentation

- Committed all chages on the local repository using:
`git commit -m ""added a new html file"`
![git-commit](./images/git-commit.png)

- Connected the local repo to the remote repo on github using:
`git remote add origin https://github.com/sukieoduwole/git-project.git` 

    Used `git remote -v` to confirm or check if there's any remote repository is linked with the local repository.
![git-remote-add](./images/git-remote-add.png)

- Pushed the local repository to the remote repo using: `git push` an error flagged off but suggested to set-upstream origin main
![git-push](./images/git-push.png)

- Set the upstream origing using:
`git push --set-upstream origin main` and got another error saying 
    > failed to push some refs to 'https://github.com/sukieoduwole/git-project.git'

    ![set-upstream](./images/set-upstream.png)

- Did a `git pull` as sugessted by the message from the above error
![git-pull](./images/git-pull.png)

    The error I got after doing a pull suggested I do a `git pull <remote> <branch>` and I used `git pull origin main` got a messasge saying 
    > Need to specify how to reconcile divergent branches.

    ![git-pull-origin](./images/git-pull-origin.png)

    Used `git config pull.rebase true` to reconcile divergent branches. 
    ![git-rebase](./images/git-rebase.png)
    This seems to solve the errors as I was able to pull the remote repo to my local repo just for me to have a consistent repo with the remote repo just for me to be able to push my local repo.

- Got an message asking to set-upstream again
![set-upstream-2](./images/set-upstream-2.png)

- Set-upstream once again using the `git push -set-upstream origin main` as suggested in the message.

![final-push](./images/final-push.png)

Finally I was able to push this local reposistory to my Github
![github](./images/github.png)








