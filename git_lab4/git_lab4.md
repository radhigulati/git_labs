## Creating a branch
Now let's create a new branch, add some commits, and merge that branch to your main branch.

> **Learning note** A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process. You can think of them as a way to request a brand new working directory, staging area, and project history. New commits are recorded in the history for the current branch, which results in a fork in the history of the project. The changes in the branches you create will not effect the main/master branch until you are ready to merge with the main/master branch.

<span style="color:red"> **TASK:** </span> Let's view all the branches available. Make sure you are in the project directory in your terminal. Use the command ```git branch``` to view all the branches. 

You should only see your ```main``` branch. Remember, we changed      ```master``` to ```main```.

<span style="color:red"> **TASK:** </span>Now, let's create a branch called ```dev```. To do this type ```git checkout -b dev```. 

<span style="color:red"> **TASK:** </span> When you type ```git branch``` you should see the ```main``` branch and the ```dev``` branch. You should also be in the ```dev``` branch. 

<span style="color:red"> **TASK:** </span> Let's access the ```demo.txt``` file within the code editor and add some changes. Type something in the file like "I love Revenue Enablemnet" or "Hello {partner}, hope you are having a nice day". Keep it appropriate for work. :) 

The change you made will not be available in the ```main``` branch yet. If you want to check and see what the ```txt``` file in the ```main``` branch looks like, you can go back to the ```main``` branch by typing the command ```git checkout main``` and viewing the ```demo.txt``` file.

<span style="color:red"> **TASK:** </span> Now we want to stage and commit the change we made to the ```demo.txt``` file in the ```dev``` branch. To do this type the ```git add .``` command then ```git commit -m "Adding the dev branch"```

<span style="color:red"> **TASK:** </span> You can verify your commit history in the new branch by typing ```git log```. Here you should see the new commit.

Right now, the ```main ``` branch is behind on one commit, so let's merge the ```dev``` branch with the ```main``` branch. 

*Continued in the next section* 
## Merging branches
<span style="color:red"> **TASK:** </span> To merge the code from the ```dev``` branch into the ```main``` branch, checkout the ```main``` branch first. So use the command ```git checkout main``` to access the ```main``` branch. 

<span style="color:red"> **TASK:** </span> Now we can use the ```merge``` command to merge branches, so type ```git merge dev```.

The merge should work, and you shouldn't see conflicts. In a real project, conflicts can happen and developers have to clear those conflicts before a merge is possible.

<span style="color:red"> **TASK:** </span> We can push these changes to GitHub now. Follow these commands

1. ```git add .```
2. ```git commit -m "merged dev with main"```
3. ```git push```

<span style="color:red"> **TASK:** </span> Your branches should now be merged! You can go to GitHub and checkout the ```demo.txt``` and make sure all of the contents are available.