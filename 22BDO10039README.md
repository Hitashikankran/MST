1. Basic local workflow: Part – 1
Related – Git basic local workflow
Main Task
1. Create a new directory and change into it.
   To create a new directory use command mkdir
   mkdir <filename>
   
2. Use the init command to create a Git repository in that directory.
  git init 
3. Observe that there is now a .git directory.
  after the git init command you can observe a .git directory  to initialize that you can use ls command 
4. Create a README file.
    to create readme file use touch readme.md
   ![image](https://github.com/Hitashikankran/MST/assets/156875388/48ef8d83-5ac0-44b5-adf2-14c45a6a33ca)

5. Look at the output of the status command; the README you created should appear as an untracked file.
   git status
   git add 
 
6. Use the add command to add the new file to the staging area. Again, look at the output of the status command.
   to check status git status
   to add file git add file 
7. Now use the commit command to commit the contents of the staging area.
    git commit -m "this is file 1"
   ![image](https://github.com/Hitashikankran/MST/assets/156875388/2637e79c-5e88-4a6a-8906-1fef9df20750)

 
8. Create a src directory and add a couple of files to it.
   to create src direc use mkdir
   to create file touch src
   vi file1.txt
   ![image](https://github.com/Hitashikankran/MST/assets/156875388/53ac2f28-54e9-4eb9-95dd-844cff9c8951)

9. Use the add command, but name the directory, not the individual files. Use the status command. See how both files have been staged. Commit them.
   git add src
   git commit -m "file1"
10. Make a change to one of the files. Use the diff command to view the details of the change.
     git diff
    ![image](https://github.com/Hitashikankran/MST/assets/156875388/6dd834c8-81f8-428f-8cd8-3ecec8559b38)

11. Next, add the changed file, and notice how it moves to the staging area in the status output. Also observe that the diff command you did before using add now gives no output. Why not? What do you have to do to see a diff of the things in the staging area? (Hint: review the slides if you can’t remember.)
 git add file 
12. Now without committing, make another change to the same file you changed in step 10. Look at the status output, and the diff output. Notice how you can have both staged and unstaged changes, even when you are talking about a single file. Observe the difference when you use the add command to stage the latest round of changes. Finally, commit them. You should now have started to get a feel for the staging area.
13. Use the log command in order to see all of the commits you made so far.
14. Use the show command to look at an individual commit. How many characters of the commit identifier can you get away with typing at a minimum?
15. Make a couple more commits, at least one of which should add an extra file.
16. ![image](https://github.com/Hitashikankran/MST/assets/156875388/5700239c-e065-4d62-8216-77a637603ade)

