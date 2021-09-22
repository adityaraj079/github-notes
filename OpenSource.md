# Guide for open source

## Study the code
The first step is always to study the code base properly

## Study the contribution guide
Second step is to study the contribution guide

## Fork the repo
Forking the repository used your username is the most important thing to do on Github

<p align="center">  <img  src="https://github.com/adityaraj079/github-notes/blob/main/Images/Fork.png">  </p>

## Clone the project 
Clone the project on your local machine to make the changes 

`
git clone <Repo_Name>
`

## Add a remote (upstream) to original project repository
Remote means the remote location of project on Github. By cloning, we have a remote called origin which points to your forked repository. Now we will add a remote to the original repository from where we had forked.
` $ cd <your-forked-project-folder> ` `git remote add upstream <Repo_Name> `
You will see the benefits of adding remote later.

## Synchronizing your fork
Open Source projects have a number of contributors who can push code anytime. So it is necessary to make your forked copy equal with the original repository. The remote added above called Upstream helps in this.
` $ git checkout main` `$ git fetch upstream` `$ git merge upstream/main` `$ git push origin main`
The last command pushes the latest code to your forked repository on Github. The origin is the remote pointing to your forked repository on github.

## Now it two parts
1. [Working on a multi branch project](#section_name)
          <a name="### Working on a multi branch project"></a>    
2.  [Working on a single branch project](#section_name)
          <a name="### Working on a single branch project"></a>    

### Working on a multi branch project
1. ` git branch `  -  Know the branch you are currently on
2. ` git branch -a ` - To know about all the branchs in the repo (Detachable ones also)
3. ` git checkout <Branch_Name> ` - To jump on your branch
4. Now make your changes on the repo
5. ` git add . ` - To add all the changes to staged 
6. ` git commit -m "<Your_Message>" ` - To make a commit message
7. ` git push origin <Branch_Name> ` - To push the changes

### Working on a single branch project
1. Work on the repo
2. ` git add . ` - To add all the changes to staged 
3. ` git commit -m "<Your_Message>" ` - To make a commit message
5. ` git push ` - To push the changes

## Push code and create a pull request
You now have a new branch containing the modifications you want in the project you forked. Now, push your new branch to your remote github fork.
`$ git push origin <feature-branch>` Now you are ready to help the project by opening a pull request means you now tell the project managers to add the feature or bug fix to original repository. You can open a pull request by clicking on green icon -

<p align="center">  <img  src="https://github.com/adityaraj079/github-notes/blob/main/Images/PR.png">  </p>


Remember your upstream base branch should be main and source should be your feature branch. Click on create pull request and add a name to your pull request. You can also describe your feature.

Fantastic! You've already made your first contribution.🥳

BE OPEN!
Happy Coding 👩‍💻👩‍💻