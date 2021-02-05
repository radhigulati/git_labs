## Create project
Let's begin!

<span style="color:red"> **TASK:** </span> First, let's create a new directory in the Terminal where we will store all projects. Make sure you are in your home directory before creating the projects folder. To check which directory you are in use the ```pwd``` command in your terminal and you should see something like ```/Users/radhika```. If you type in ```pwd``` into your terminal you should see the current directory you are in.

<span style="color:red"> **TASK:** </span>Once you are in the correct directory use the command ```mkdir projects``` to create a new projects folder. Type in the command ```ls -la``` to list out the contents of this folder. 

<span style="color:red"> **TASK:** </span> Let's access the new projects folder. To do this type in the command ```cd projects```. If you type in ```pwd``` you should see something like ```/Users/radhika/projects```.

<span style="color:red"> **TASK:** </span> Now lets create a directory for our project using the ```mkdir``` command and the directory name. One person should name their project ```git-demo``` and one person should name their project ```git-demo-rko```. I will use ```git-demo``` in my examples in this tutorial. 
```
$ mkdir git-demo
```
<span style="color:red"> **TASK:** </span> Now let's access the directory using the ```cd``` command
```
$ cd git-demo
```
<span style="color:red"> **TASK:** </span> If you type in ```pwd``` you should see that you are in the ```git-demo``` folder.

<span style="color:red"> **TASK:** </span> We need it initialize this repository by using the command ```git init```. Make sure you are in your project folder, and type ```git init``` into your terminal. 
> **Learning Note** Executing git init creates a .git subdirectory in the current working directory, which contains all of the necessary Git metadata for the new repository.

> **Learning Note** You won't see anything in GitHub right now because we haven't pushed anything to GitHub. We've just been working on the local machine, so everything is stored locally right now.

## Create your first file
Let's create a a file in the project folder called ```demo.txt```.

<span style="color:red"> **TASK:** </span> To create this file, type ```touch demo.txt``` into your terminal.

Let's open the code editor you downloaded earlier for this project. <span style="color:red"> **TASK:** </span> To open VScode from the project folder in the terminal, you can type ```code .``` within your terminal within the project. Once your code editor is open, you should have access to your file. <span style="color:red"> **TASK:** </span> Within your file write ```This is a demo git repo.``` Save the changes once written (```cmd + s``` or ```file``` > ```save```)

Let's add this file to our staging area. 

> **Learning Note** The staging area is where we keep track of all the files we need to commit. If a file is not added to the staging area, it will not be commited. 

> **Learning Note** The ```git add``` command adds a change in the working directory to the staging area. It tells Git that you want to include updates to a particular file in the next commit. However, ```git add``` doesn't really affect the repository in any significant way—changes are not actually recorded until you run git commit.

<span style="color:red"> **TASK:** </span>To add a file to the staging area  type in the command ```git add demo.txt```. If you want to add all the files to the staging area you can use ```git add .``` For our case right now, you can use either.

## Commit changes
<span style="color:red"> **TASK:** </span> Now let's commit the changes. Type ```git commit -m "First commit. Added demo.txt file"```

Then type ```git status``` to check the status of git.