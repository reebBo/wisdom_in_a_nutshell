npm init to initialize package.json
npm i gh-pages
in package.json add the "homepage" line
create a script to be able to deploy to gh pages repo 
(dist is the folder to deploy)


 "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "deploy": "gh-pages -d dist"
  },
  "author": "reeb",
  "license": "ISC",
  "homepage": "https://reebBo.github.io/wisdom_in_a_nutshell",
  "dependencies": {
    "gh-pages": "^3.1.0"
  }

create .gitignore in the root folder of your project(on the comp) and add there node_modules
create repo in github, then:

git init 
git commit -m "first commit"
git remote add origin https://github.com/reebBo/wisdom_in_a_nutshell.git
git push -u origin master

under the brances dropdown on github we only have master branch. No gh-pages. To deploy to gh-pages:
npm run deploy
 (under the brances dropdown we will find now the gh-pages)


on github- on the page of the project just pushed, go to settings

under GitHub pages, gh-pages branch is already selected
and there is a message:
  Your site is published at https://reebbo.github.io/wisdom_in_a_nutshell/



  https://www.youtube.com/watch?v=SKXkC4SqtRk 