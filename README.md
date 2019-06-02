
# Windows 10

Instalirati git

https://www.onlinetutorialspoint.com/git/how-to-install-git-windows-10-operating-system.html
https://gitforwindows.org/

Instalirati nodejs

https://blog.risingstack.com/node-js-windows-10-tutorial/

Notice: Ako je  bio otvoren git-bash zatvoriti i otvoriti novi prozor. 
		U protivnom 'git-bash' nece prepoznati da je nodejs instaliran.

 npm --version
6.9.0

 node --version
v10.16.0

 
 
https://www.tutorialspoint.com/gulp/gulp_installation.htm

### Bash basics
cd .. </-- Go back
cd [ENTER] </-- Goes back to Home folder path on PC(alias: ~)
cd /c/$FOLDER_PATH 
ls
ll

#####

Instaliranje GULP-a globalno

npm install gulp -g
npm install gulp-cli -g

#####

cd
mkdir Sites
cd Sites
mkdir $PROJECT_FOLDER_NAME // OR // git clone $REPO_URL $PROJECT_FOLDER_NAME
cd $PROJECT_FOLDER_NAME

npm init

#### Gulp vezba


#### Create gulpfile.js


	//  Require Gulp into file and define the variable
	var gulp = require('gulp');

	//  Run the example task, if installed correctly and "gulp hello" is ran, an greeting message should be printed in the logs
	gulp.task('hello', function() {
	     console.log('Hello World!');
	});

########

npm install gulp
npm link gulp // U slucaju da izbaci error, moramo ga linkovati na globalnu instalaciju

> npm ERR! code EINVALIDTAGNAME
> npm ERR! Invalid tag name "gulp": Tags may not have any characters that encodeURIComponent encodes.


gulp


#### git clone mci-starter

//  Require Gulp into file and define the variable
var gulp = require('gulp');

//  Run the example task, if installed correctly and "gulp hello" is ran, an greeting message should be printed in the logs
gulp.task('hello', function() {
     console.log('Hello World!');
});







