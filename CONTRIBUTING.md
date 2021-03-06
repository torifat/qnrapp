## Contributing (Step-by-step)

1. Clone the Repo:

        git clone git@github.com:qnr-bangladesh/qnrapp.git

2. Create a new Branch:

        cd qnrapp
        git checkout -b new_qnrapp_branch

 > Please keep your code clean: one feature or bug-fix per branch. If you find another bug, you want to fix while being in a new branch, please fix it in a separated branch instead.

3. Code
  * Adhere to common conventions you see in the existing code
  * Include tests, and ensure they pass

4. Follow the Coding Conventions

5. Commit

  For every commit please write a short (max 72 characters) summary in the first line followed with a blank line and then more detailed descriptions of the change. Use markdown syntax for simple styling.

  **NEVER leave the commit message blank!** Provide a detailed, clear, and complete description of your commit!

6. Update your branch

  ```
  git fetch origin
  git rebase origin/master
  ```

7. Fork

  ```
  git remote add mine git@github.com:<your user name>/qnrapp.git
  ```

8. Push to your remote

  ```
  git push mine new_qnrapp_branch
  ```

9. Issue a Pull Request

  Before submitting a pull-request, clean up the history, go over your commits and squash together minor changes and fixes into the corresponding commits. You can squash commits with the interactive rebase command:

  ```
  git fetch origin
  git checkout new_qnrapp_branch
  git rebase origin/master
  git rebase -i

  < the editor opens and allows you to change the commit history >
  < follow the instructions on the bottom of the editor >

  git push -f mine new_qnrapp_branch
  ```


  In order to make a pull request,
  * Navigate to the qnrapp repository you just pushed to (e.g. https://github.com/your-user-name/qnrapp)
  * Click "Pull Request".
  * Write your branch name in the branch field (this is filled with "master" by default)
  * Click "Update Commit Range".
  * Ensure the changesets you introduced are included in the "Commits" tab.
  * Ensure that the "Files Changed" incorporate all of your changes.
  * Fill in some details about your potential patch including a meaningful title.
  * Click "Send pull request".

  Thanks for that -- we'll get to your pull request ASAP, we love pull requests!
