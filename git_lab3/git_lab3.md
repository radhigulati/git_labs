## Add project to GitHub

<span style="color:red"> **TASK:** </span>Let's navigate to GitHub and create a new project. Within GitHub, navigate to the ```new``` button to create a new project. For the ```repository name``` use ```git-demo```. You can add a description that says ```This project is a beginner git project.``` Make the project ```public```. DO NOT initialize this project with a ```README file```. Then click ```create repository```.

You have now created an empty repository with a README file within GitHub. You will be directed to a page with some instructions that I will describe below. Keep in mind we've already run ```git init```.

<span style="color:red"> **TASK:** </span> You have already added and commited changes to Git, so type ```git status``` to check the status of git. If you have changes that have not been added run the add and commit commands again:

    git add .
    git commit -m "add some description"

If you see:

    Your branch is up to date with 'origin/main'.

    nothing to commit, working tree clean
This means you have not made any new changes.

<span style="color:red"> **TASK:** </span> Now, we need to point our local repository to the remote repository. To do that type the following command in your terminal (make sure you are in your project directory)
```git remote add origin [repository url]```

The ```repository url``` will be ```git@github.com:[your github username]/[name of repo].git```. For example, my url would be ```git@github.com:radhigulati/git-demo.git```. You can find this url in the instructions on your GitHub page for the new project you created. 

<span style="color:red"> **TASK:** </span>You can change the ```master``` branch to ```main``` by using the command ```git branch -M main```. If you are interested in why GitHub renamed it's ```master``` branch to ```main``` checkout [this](https://www.theserverside.com/feature/Why-GitHub-renamed-its-master-branch-to-main#:~:text=GitHub%20took%20action%20based%20on,a%20different%20default%20for%20new) article.

**If you recieve an error that says ```error: refname refs/heads/master not found
fatal: Branch rename failed``` then follow the steps below otherwise skip these steps:**

1. Within the project directory, type the command ```cd .git```
2. Then open this folder in your code editor (with vscode you can type in ```.code```)
3. Navigate to the ```HEAD``` file 
4. Change ```ref: refs/heads/master``` to ```ref: refs/heads/main```
5. Save this file

Now your ```master``` branch will be ```main```.

<span style="color:red"> **TASK:** </span> Let's push your project to GitHub. To do this, type the command ```git push -u origin main```.

If you navigate to GitHub, you should see your file in GitHub!