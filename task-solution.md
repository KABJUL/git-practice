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

