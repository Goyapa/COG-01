# Node and NPM Commandline 

## Node Commands
[Node.js](https://nodejs.org/en/)

Command                     |   Explanation
-------------------------   |   ----------------
$ node -v                   |   show node version
|   |   |
$ node [file]               |   run file with node
$ node 01-server.js         |   run server.js with node
|||
$ node                      |   run node [REPL](https://nodejs.org/dist/latest-v4.x/docs/api/repl.html) see [REPL Driven Development](http://thinkingonthinking.com/scripting-a-csv-converter/) (RDD)
> fs = require('fs');       |   require [File System module](https://nodejs.org/dist/latest-v4.x/docs/api/fs.html)
fs.readFile('./movies.csv', function(e, data) { |   call fs.readfile(), you nead a movies.csv file
... console.log(data);      |   log data
... })                      |   close function
undefined                   | no return value
> \<Buffer 74 69 74 6c 65 3b ...>   |  is what the REPL will answer


## Node Package Manager(NPM) Commands
[NPM websearch](https://www.npmjs.com/)

Command                     |   Explanation
----------------------------|   ----------------
$ npm list                  |   list of installed packages
$ npm install [packageName] |   install package into node_modules folder
$ npm install underscore    |   install underscore into current folder
|   |   |
$ npm uninstall [packageName] |   uninstall package into local folder
$ npm uninstall underscore    |   uninstall underscore into current folder
|   |   |
$ npm search [keyword keyword] | search packages with keywords
$ npm search comment json     |   search for comment-json



[Node.js reference Cards](https://dzone.com/refcardz/nodejs) 


[Introduction to npm](http://modernweb.com/2014/03/31/introduction-to-npm/?ref=dzone)

## package.json

[AN INTERACTIVE GUIDE](http://browsenpm.org/package.json)

[Creating Node.js modules](https://docs.npmjs.com/getting-started/creating-node-modules)

[Using a package.json](https://docs.npmjs.com/getting-started/using-a-package.json)

[Specifics of npm's package.json handling](https://docs.npmjs.com/files/package.json)

Command                     |   Explanation
----------------------------|   ----------------
$ npm init                  | create a package.json
npm install [packageName] --save  | saves package version into package.json dependencies
npm install foo --save  | { "dependencies" : { "foo" : "2.0.1"}}
npm install [packageName] --save-dev  | saves package version into package.json devdependencies
npm install bar --save-dev  | "devDependencies": {"bar": "~1.6.3"}


* npm install   will install both "dependencies" and "devDependencies"

* npm install --production  will only install "dependencies"

* npm install --dev   will only install "devDependencies"


[How to set NODE_ENV to production/development](http://stackoverflow.com/questions/9198310/how-to-set-node-env-to-production-development-in-os-x): Have also a look at the posts of "walkerbe" and "Lukas Liesis"

[EnvironmentVariables](https://help.ubuntu.com/community/EnvironmentVariables)

[Setting environment variables in node.js](http://stackoverflow.com/questions/22312671/node-js-setting-environment-variables/28821696#28821696)

