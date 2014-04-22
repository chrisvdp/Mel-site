Mel-site
========



all commands that appear as code style should be run from the terminal.

Setup (first time only)
---
install [nodejs](http://nodejs.org/)
install grunt-cli
```
npm install -g grunt-cli
```

clone this repo

```
git clone <clone url on the right>
```

Install dependancies 
```
npm install
bower install
```

Working with the site
---

Uncompiled changes are in the app folder, make changes to files in this folder and then follow the instructions below. Don't make changes in the dist folder as they will be overridden. 

preview the site (local changes preview)
```
grunt serve
```
Build the site (prep to go live)
```
grunt
```
grunt serve will compile the site and serve it locally. Run it if you are editing the site.
When all changes are done and you want it to go live, run grunt and push to git.

Push to github
---
the commit command will not push the site live, so you can run this command for each set of changes you make. Change the commit message to reflect the changes you made, ie "updated title tag". 
```
git commit -am  "<commit message>"
```

To push the site live run the subtree push command. The changes in the dist folder will display on the live site.
```
git subtree push --prefix dist origin gh-pages
```
