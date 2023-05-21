# Gym Git Exercise Solutions

## Bundle 1
### Exercice 1
Here's how i did it:

1. Create a Project & Initialize Git:
- Create a new directory for my project: `mkdir Gym-Git-Exercise-Solutions`
- Change into the project directory: `cd Gym-Git-Exercise-Solutions`
- Initialize Git: `git init`

2. Rename my main branch from `master` to `main`:
- Rename the branch locally: `git branch -m master main`

3. Make changes to the project

5. Stage my changes and commit them:
- Add all changes to the staging area: `git add .`
- Commit the changes with a descriptive message: `git commit -m "Gym-Git-Exercise-Solutions init"`

6. Create a GitHub repo called `Gym-Git-Exercise-Solutions` and connect it with the project
- Add the remote repository URL: `git remote add origin https://github.com/Muhindo-Galien/Gym-Git-Exercise-Solutions`
- Push the main branch to the remote repository: `git push -u origin main`

7. Create a new branch dev:
- Create the dev branch locally: `git branch dev`
- Switch to the dev branch: `git checkout dev`

8. From dev, create another branch test:
- Create the test branch from dev: `git checkout -b test`
- Go back to the dev branch and delete the test branch:
- Switch back to the dev branch: `git checkout `dev
- Delete the test branch: `git branch -D test`

## Bundle 1
### Exercice 2

1. Create a new home.html file and add some HTML changes:
- `touch home.html`
- Open `home.html`  in a text editor and make changes
2. Save the changes to the home.html file:
- `git add home.html`
3. Stash save my current changes:
- `git stash save`
4. Repeat the process for a new about page
- `touch about.html`
- Open `about.html` in a text editor and make the necessary changes
- `git add about.html`
- `git stash save`
5. Repeat the process for a new team page:
- `touch team.html`
- Open `team.html` in a text editor and make the necessary changes
- `git add team.html`
- `git stash save`
6. Using stash pop, restore the changes of the about page:
- `git stash pop stash@{1}`
7. With the help of an index, use stash pop to bring back the home page changes:
- `git stash apply stash@{0}`
8. Commit the current changes and push them:
- `git add .`
- `git commit -m "home and aboout page added"`
- `git push origin dev`
9 .Using stash pop, restore the changes of the team page:
- `$ git stash pop stash@{1}
10. Reset the current changes using git reset to go back to the changes without the team page:
- `$ git reset --hard HEAD`

## Bundle 2
##Exercises 1

1. Create a new branch named ft/bundle-2:
- `git checkout -b ft/bundle-2`
2. Add new changes to my project. Create a new page named services.html and add some changes:
- `touch services.html`
- Open services.html in a text editor and make the necessary changes
3. Commit my changes:
```bash
git add services.html
git commit -m "services page added"
```
4. Push my branch to the remote repository:
- `$ git push origin ft/bundle-2`
5. Create a Pull Request against the main branch in my GitHub repository.
