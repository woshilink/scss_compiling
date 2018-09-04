# scss_compiling
A simple  way to compile scss.

source:
https://webdesign.tutsplus.com/tutorials/watch-and-compile-sass-in-five-quick-steps--cms-28275

Steps to build

- Install Node.js

- Initialize NPM

- Install Node-Sass
  npm install node-sass
  
- Write Node-sass Command
  Open the package.json file
  In the scripts section add an scss command, under the test command, as it’s shown below:
  
  "scripts": {
  "test": "echo \"Error: no test specified\" && exit 1",
  "scss": "node-sass --watch scss -o css"
  }

  When we run this script it will watch every .scss file in the scss/ folder, then save the compiled css in css/ folder every time we change a .scss file.

- Run the Script
  npm run scss
