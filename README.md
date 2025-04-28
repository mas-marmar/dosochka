pwd

mkdir mashashadow

cd mashashadow/

git init

git status

git remote add https://github.com/mas-marmar/dosochka.git

git remote -v

touch README.md

explorer .

git add .

git commit -m "dh"

git config --global user.name "da"

git config --global user.email "masamaslakova@gmail.com"

git commit -m "dh"

git status

git remote -v
origin  git@github.com:mas-marmar/dosochka.git~ (fetch)
origin  git@github.com:mas-marmar/dosochka.git~ (push)

git remote remove origin

git remote -v

git remote add origin https://github.com/mas-marmar/dosochka.git

git push -u origin master

npx create-strapi-app dosochka --quickstart
