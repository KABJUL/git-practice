# I CAN WIN

## 1. Install Git and generate a pair of SSH keys. Authorize the public key on GitHub.

ssh-keygen -t rsa -C "kabodi.julia@gmail.com"

## 2. Specify your user.name and user.email in git.

git config --global user.name "KABJUL"

git config --global user.email "kabodi.julia@gmail.com"

## 3. Create a new repository on github.com and clone it locally to your computer.

cd /d/GitProjects/

git clone git@github.com:KABJUL/git-practice.git

## 4. Create a file called song.txt and put there half the text of your favorite song.


## 5. Make a commit called "add first half of my favorite song" and send it to the server.

git add song.txt

git commit -m “add first half of my favorite song”

## 6. Make sure github has a song.txt file with the lyrics.

git push

## 7. Using the github's web interface, add the second half of the lyrics and make a commit with the name "finish my song".


## 8. Make a pull in the local repository and make sure that the commit you created on github is pulled up and you have all the lyrics.

git pull

# BRING IT ON

This task is performed immediately after the previous one (I Can Win).
## 1. Add a .gitignore file to the project and configure it to hide files with the extension .db, .log and directories with the names target or bin.

cd /d/GitProjects/git-practice
touch .gitignore
    *.db
    *.log
    target/
    bin/

## 2. Create a feature branch and add two commits to it

git checkout -b feature
git add song.txt
git commit -m ""
git add song.txt
git commit -m ""

## 3. Merge the feature branch in master

git checkout main
git merge feature

## 4. Return to feature and create the arrows.txt file with the following contents:
The ship glides gently on the waves
As day turns into night

Make a commit.

git checkout feature
git add arrows.txt
git commit -m "Add first two lines to arrows"

## 5. Go to master. Create the arrows.txt file there and add the following text:
One thousand burning arrows
Fill the starlit sky

Make a commit.

git checkout main
git add arrows.txt
git commit -m "Add last two lines to arrows"

## 6. Merge feature in master resolving the conflict: save all 4 lines in arrows.txt file in the order they were added in steps 4 and 5.

git merge feature
git add arrows.txt
git commit -m ""
git push
git push -u origin feature