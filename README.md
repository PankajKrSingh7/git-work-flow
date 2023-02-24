
# DESCRIPTION 
Create a branching model to help team understand the Git Feature Branch Workflow for faster and efficient integration of work



### Working on feature2 
=======
changes in feature 2 for update

merging feature2 into Integration Branch


### Working on Feature1
=======
merging feature1 into HotFix
merging feature1 into Integration
merging feature1 into Production

### making some changes into Hotfix before merging into Integration and Production



# Steps taken-


## Step1 : Creating repository and Initialising Branches
```
mkdir git-work-flow
cd git-work-flow
git init
```
 
 
 ### Adding a readme file (Default editor  : VS Code)
  ```
touch README.md
git add README.md
git commit -m "First Commit"
  ```
 
 ### Creating HotFix  and integration Branch
 ```
git branch HotFix
git branch Integration
```

## Step2 :  Creating Feature1 and Feature2 Branches
```
git branch Feature1
git Branch Feature2
```

## Step3 : Making changes in Feature2 , Creating pull Request and merging it to Integration Branch
```
vi README.md
```
### Creating pull request using Github
```
```
### Merging with Integration
```
git checkout Integration
git merge --no-f Feature2

git branch --delete Feature2
```

## Step4 : Committing some changes in Feature1 and rebase it to Integration Branch
```
vi README.md
git add 
git commit -m "Changes in Feature1"
git checkout Feature1
git rebase Integration
```

## Step5 : Create Pull Request, add 2 reviewers, get the PR reviewed & Merge the Integration branch into Hotfix and Production branch to update these branches
```
git checkout Integration
--creating pull request using GitHub

git checkout Hotfix
git merge Integration

git checkout Production
git merge Integration

git status

```

## Step6 : Commit some changes in Feature 1 branch, and then Create Pull Request, add 2 reviewers,get the PR reviewed & merge it into Integration, Hotfix, and Production branch. Delete this branch once merging is complete
```
vi README.md
git add 
git commit -m "Changes in Feature1"
git checkout Feature1
--creating pull request using github

git checkout Hotfix
git merge Feature1

git checkout Production
git merge Feature1

git checkout Integration
git merge Feature1

git branch --delete Feature

```

## Step7 : Commit some changes in the Hotfix branch and Create Pull Request, add 2 reviewers, get the PR reviewed & merge it into the Production as well as the Integration branch
```
vi README.md
git add 
git commit -m "Changes in Hotfix"

git checkout Hotfix
creating pull request using github

git checkout Production
git merge Hotfix

git checkout Integration
git merge Hotfix

```

Note - I have done PR reviews using Github UI


## Commit History and Graph
<img width="1440" alt="Screenshot 2023-02-24 at 12 21 00 PM" src="https://user-images.githubusercontent.com/54628129/221112387-da55702b-76f0-4a51-9c5d-ff28909171ec.png">




