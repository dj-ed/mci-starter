
# Windows 10

Instalirati git i  git-bash koji dolazi sa instalacijom.
https://gitforwindows.org/
https://www.onlinetutorialspoint.com/git/how-to-install-git-windows-10-operating-system.html


Instalirati nodejs

https://blog.risingstack.com/node-js-windows-10-tutorial/
Proveriti da li su instalirani *npm* in *nodejs*.
Notice: Ako je  bio otvoren git-bash zatvoriti i otvoriti novi prozor. 
		U protivnom 'git-bash' nece prepoznati da je nodejs instaliran.
```
 npm --version
6.9.0
 node --version
v10.16.0
```

#### git-bash basics
```
cd ..  </-- Folder nazad
cd     </-- Home folder na računaru(alias: ~)
cd /c/$FOLDER_PATH
ls       </-- Prikazuje sadrzaj trenutne putanje 
ll       </-- Prikazuje sadrzaj trenutne putanje sa dodatnim informacijama
```

#### Gulp instalacija
https://www.tutorialspoint.com/gulp/gulp_installation.htm
Instaliranje GULP-a globalno
```
npm install gulp -g
npm install gulp-cli -g
```

##### Gulp vezba

cd
mkdir Sites
cd Sites
mkdir $PROJECT_FOLDER_NAME // OR // git clone $REPO_URL $PROJECT_FOLDER_NAME
cd $PROJECT_FOLDER_NAME

1. Prvo kreiramo *package.json*:
```
npm init
```

2. Zatim kreiramo **gulpfile.js** sa sledecim sadrzajem

```
	//  Require Gulp into file and define the variable.
	var gulp = require('gulp');
	// 'hello' task definition.
	gulp.task('hello', function() {
	     console.log('Hello World!');
	});
```

3. U git-bash zatim instaliramo gulp lokalno u projekat pomocu sledece komande
```
npm install gulp
npm link gulp </-- U slucaju da izbaci error(> npm ERR ! Invalid tag name "gulp":), moramo ga linkovati na globalnu instalaciju
```

Pokrenuti *hello* gulp task koji smo definisalu unutar **gulpfile.js**
```
gulp hello
```

###### Ako je instalacija prosla uspeshno klonirati *'mci-starter'* lokalno i instalirati ga gore koriscenim principom.
###### Unutar projekta trenutno samo postoji 'default' task koji se moze pokrenuti sa komandom:
```
gulp
```







