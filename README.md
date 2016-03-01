To launch the kit you should run this commands:
- npm install
- bower install
- gulp

###### All sources files must be placed in /src directory.

*****

To update packages you need to install https://www.npmjs.com/package/npm-check-updates and run `npm run updatePack` in a project folder. 

*****

### Auto regression test manual:
1. Run `sudo npm install phantomjs` or `brew install phantomjs`
2. Run `phantomjs -v` if all works
3. Run `sudo npm install -g casperjs` and `casperjs`
4. Check if BackstopJS is installed and run `npm install` in this folder
5. Run `gulp genConfig` in BacktopeJs folder. It should create config file in a project root folder.
6. Run task `gulp reference` to create initial pack, then after changes you can see diffs with `gulp test` 