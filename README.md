Mel-site
========

site for mel

install [nodejs](http://nodejs.org/)
clone this repo

run and build the site
```
npm install
bower install
grunt serve
grunt
```
grunt serve will compile the site and serve it locally. Run it if you are editing the site.
When all changes are done and you want it to go live run grunt and push to git.

Push to git
```
git commit -am  "<commit message>"
git subtree push --prefix dist origin gh-pages
```
