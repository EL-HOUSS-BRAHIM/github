# github Tasks:

## Task 2: Create a new github repository
```bash
git clone https://github.com/EL-HOUSS-BRAHIM/github.git
cd github
git branch -m master
```
![github Task2](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github1.png?raw=true?raw=true)

---

## Task 3: Create Task1 folder in the master branch and push ./Task1/README.md file.
```bash
mkdir Task1
touch Task1/README.md
git add .
git commit -m "adding Task1 folder and the README file on the master branch"
git push origin master
```
![github Task3](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github2.png?raw=true)

---

## Task 4: Create a new dev branch and push a test file.
```bash
git checkout -b dev
touch test
git add .
git commit -m "adding test file to the dev branch"
git push --set-upstream origin HEAD
```
![github Task4](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github3.png?raw=true)

---

## Task 5: Create a new branch %USERNAME-new_feature.
```bash
git checkout -b %USERNAME-new_feature
```
![github Task5](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github4.png?raw=true)

---

## Task 6: Add README.md to %USERNAME-new_feature branch.
```bash
touch README.md
```
![github Task6](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github5.png?raw=true)

---

## Task 7: Check repository status using git status.
```bash
git status
```
![github Task7](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github6.png?raw=true)

---

## Task 8: Add .gitignore file to ignore files starting with .
```bash
echo ".*" > .gitignore
```
![github Task8](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github7.png?raw=true)

---

## Task 9: Commit and push changes to the github repo.
```bash
git add -f .
git commit -m "adding readme and gitignore file %USERNAME-new_feature"
git push --set-upstream origin HEAD
```
![github Task9](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github8.png?raw=true)

---

## Task 10: Create a Merge Request (MR) to the dev branch.
```bash
#No commands here!
```
![github Task10](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github.png?raw=true)

---

## Task 11: Merge %USERNAME-new_feature with dev and create an MR to master. Merge dev with master.
```bash
git checkout dev
git merge %USERNAME-new_feature
git push origin HEAD

git checkout master
git branch --unset-upstream
git merge dev
git push origin HEAD
```
![github Task11-1](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github9.png?raw=true)
![github Task11-2](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github10.png?raw=true)

---

## Task 12: Checkout %USERNAME-new_feature, make changes to README.md, commit, and revert the last commit.
```bash
git checkout %USERNAME-new_feature
echo "this the New readme.md on the %USERNAME-new_feature branch" > README.md
git add .
git commit -m "editing the README file on the %USERNAME-new_feature branch"
git revert HEAD
```
![github Task12](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github11.png?raw=true)

---

## Task 13: Check the repo with git log, create log.txt in master, and save git log output.
```bash
git checkout master
git log
git log > log.txt
git add log.txt
git commit -m "Save git log output to log.txt"
git push origin HEAD
```
![github Task13](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github12.png?raw=true)

---

## Task 14: Delete local and remote %USERNAME-new_feature branch.
```bash
git branch -D %USERNAME-new_feature
git push origin --delete %USERNAME-new_feature
```
![github Task14](https://github.com/EL-HOUSS-BRAHIM/git/blob/images/images/github13.png?raw=true)

---

## Task 15: Add all used commands to git_commands.md in the dev branch.
```bash
#No commands on this step!
#This file is task 15
```

