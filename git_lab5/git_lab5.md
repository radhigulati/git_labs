## Creating a Pull Request
Let's learn about pull requests.

You are going to make a pull request on your partners ```git-demo``` project. 

<span style="color:red"> **TASK:** </span> Go to their project and click the ```fork``` button at the top right. Make sure you fork the project to your own organization. To clarify, you may see two organizations: yours and CircleCI. Make sure you click on your organization.

> **Learning note** Forking will save the project to your GitHub account (you should see the project once it's forked).

*Do the task below in the projects directory. Your path should look like /Users/radhika/projects*

<span style="color:red"> **TASK:** </span> Now, clone the repo locally (in your terminal). This link is available in GitHub when you click on the code button in the repo and choose ssh (you just need to use ```git clone``` before the url). For example 

    $ git clone git@github.com:radhigulati/git-demo.git

<span style="color:red"> **TASK:** </span> Create a new branch with ```git checkout -b <your-name demo>``` For example, ```git checkout -b radhika-demo```

<span style="color:red"> **TASK:** </span> Create a new remote for the upstream repo with the command:

```git remote add upstream <link to github url>``` 

The GitHub url is your partners GitHub project url.

For example: ```git remote add upstream https://github.com/radhigulati/git-demo-rko```

> **Learning note** "Upstream repo" refers to the original repo/parent repo you created your fork from.

<span style="color:red"> **TASK:** </span> Type ```ls -la``` into the terminal and you should see the ```demo.txt``` file. Make sure you see text from you partner. Within the file, you can type in something to them! (like "we love revenue enablement" or "Hello, {partner_name}!). Again, keep it safe for work. :) 

<span style="color:red"> **TASK:** </span> Double check you are in your branch with the command```git branch```. When you type this command, you should see your branch highlighted.

<span style="color:red"> **TASK:** </span> Follow the steps below to push your new changes. For instruction 3, ```[branch]``` will be the branch name that you used without the brackets. For example ```git push -u origin radhika-demo```:

1. ```git add demo.txt```
2. ```git commit -m "added my comment for a PR"```
3. ```git push -u origin [branch]``` ex: ```git push -u origin radhika-demo```

<span style="color:red"> **TASK:** </span> Go to the GitHub project page, and click on ```pull requests```.

<span style="color:red"> **TASK:** </span> You should see a green button that says ```New Pull Request``` that you should click on.

<span style="color:red"> **TASK:** </span> Add a description of what the PR contains, and click on ```create pull request```


## Accepting a Pull Request
<span style="color:red"> **TASK:** </span> Each person should go to ```pull requests```, click on the ```pull requests```, and as long as there are no conflicts you can ```merge the pull request```.

## Congrats
You have finished the Git tutorial!

In this tutorial, you learned how to:
* Use the command line
* Create and manipulate directories and files
* Commit and push changes to GitHub from the command line
* Create and accept pull requests

Next, we will work on a coding project where you will use the skills you learned today.