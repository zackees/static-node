# template-python-cmd
A template for quickly making a python lib that has a command line program attached

[![Linting](../../actions/workflows/lint.yml/badge.svg)](../../actions/workflows/lint.yml)

[![MacOS_Tests](../../actions/workflows/push_macos.yml/badge.svg)](../../actions/workflows/push_macos.yml)
[![Ubuntu_Tests](../../actions/workflows/push_ubuntu.yml/badge.svg)](../../actions/workflows/push_ubuntu.yml)
[![Win_Tests](../../actions/workflows/push_win.yml/badge.svg)](../../actions/workflows/push_win.yml)

Replace `template-python-cmd` and `template_python_cmd` with your command. Run tox until it's
correct.

## instructions for portable node

https://codyswartz.us/wp/finds/node-js-stand-alone-portable-with-npm


« What ways are there to find out how my computer was hacked?
Squeezing The Space Out Of Your SSD with Windows 8 »
Node js Stand Alone Portable with NPM
By Cody Swartz | Published: September 22, 2015
If you want to directly download node.exe (all distributions here) and run it by itself, including the infamous Node Package Manager NPM; here are the steps I took to accomplish this. This also applies to environments where you have restricted permissions and do not have administrative permissions. In such an instance you cannot use the installer which requires administrative permissions and would otherwise set up the PATH variable in Windows – which you cannot change anyways without admin permissions.

This all originated from the error: “npm should be run outside of the node repl, in your normal shell.”
Which I answered here at StackOverflow:
http://stackoverflow.com/questions/24476805/how-to-resolve-npm-should-be-run-outside-of-the-node-repl-in-your-normal-shell/31148216#31148216

![image](https://github.com/zackees/static-node/assets/6856673/23f1ecea-3db0-424f-b864-0bfff427ac5a)


Here’s what I did for Windows
Download the node.exe stand-alone from nodejs.org
Downloads page
All latest distributions
Grab an NPM release zip off of github
https://github.com/npm/npm/releases
Create a folder named: node_modules in the same folder as node.exe
Extract the NPM zip into the node_modules folder
Rename the extracted npm folder to npm and remove any versioning ie: npm-3.3.4 –> npm.
Copy npm.cmd out of the /npm/bin/ folder into the root folder with node.exe
Open a command prompt in the node.exe directory (shift right-click “Open command window here”)
Now you will be able to run your npm installers ie:
npm install -g express
npm install express --save
Running the installers through npm will now auto install packages where they need to be located (node_modules and the root)

Don’t forget, you will not be able to set the path variable if you do not have proper permissions. So your best route is to open a command prompt in the node.exe directory to run commands (shift right-click “Open command window here”)

This entry was posted in Interesting Finds, Web Development, Windows and tagged express js, install, Node Package Manager, node.js, npm, portable, run, Windows. Bookmark the permalink. Post a comment or leave a trackback: Trackback URL.
One Trackback
By Tired of node/npm and Composer and Git installations (??) | PipisCrew Official Homepage on February 12, 2017 at 11:26 am
[…] ##ref urls used : https://gist.github.com/massahud/321a52f153e5d8f571be https://codyswartz.us/wp/finds/node-js-stand-alone-portable-with-npm […]


https://github.com/zackees/static-node



To develop software, run `. ./activate.sh`

# Windows

This environment requires you to use `git-bash`.

# Linting

Run `./lint.sh` to find linting errors using `pylint`, `flake8` and `mypy`.
