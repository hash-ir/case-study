# COVID-19 Case Study
Case Study for Data Analysis &amp; Visualization in R

## Dataset
Download the dataset from [here](https://www.kaggle.com/kimjihoo/coronavirusdataset). Please don't push or upload the dataset in the repository. If necessary, create a `.gitignore` file in the main branch (or your working branch) and write the data directory in it.    

## Setup
As discussed in the meeting, we can work on the Case Study by creating separate branches off of main branch or work in the main branch by creating separate directories. For conflict-free changes, here are both the steps:

### Create a separate branch (from main)
1. Before working or creating a branch, make sure to pull the recent changes from the repository.
```bash
git pull
```
If any change is made in the main branch, switch to the main branch `git checkout master` and then pull otherwise pull from your working branch `git checkout <yourname>`.

2. Create a new branch with your name. 
```bash
git branch <yourname>
```
Check if it is created by writing `git branch`

3. Switch to the created branch.
```bash
git checkout <yourname>
```
4. Commit and push the changes. Make sure you are switched to your branch (not the main) when you commit the changes.
```bash
git add <filenames>
git commit -m "commit message"
git push
```
If you are pushing for the first time, it might throw an error for the created branch. Use the following to set tracking of your branch with origin
```bash
git push --set-upstream origin <yourname>
# or
git push -u origin <yourname>
```
5. Merging the branches with master (for later). Once we agree on some work, we can merge the changes back to main.
```bash
git checkout main
git merge <yourname>
git push
```

### Create a directory (in main)
1. Create a directory with your name (in the main branch)
2. Add files inside the directory
3. Commit and push the changes (in the main branch)