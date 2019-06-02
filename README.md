
# Windows 10

Instalirati `git` i  `git-bash` koji dolazi sa instalacijom.

https://gitforwindows.org/
https://www.onlinetutorialspoint.com/git/how-to-install-git-windows-10-operating-system.html


Instalirati `nodejs`

https://blog.risingstack.com/node-js-windows-10-tutorial/

Ispratiti korake unutar tutorial-a i posebno obratiti paznju na dodavanje nove putanje na `Paths` windows varijablu.
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
Poenta vezbe je kreirati novi projekat i setovati osnovno frontend okruženje. Svi npm moduli ce biti instalirani unutar *node_modules* foldera a informacije o svima njima ce biti sadržane unutar *package.json* fajla.
```
cd
mkdir Sites
cd Sites
mkdir $PROJECT_FOLDER_NAME // OR // git clone $REPO_URL $PROJECT_FOLDER_NAME
cd $PROJECT_FOLDER_NAME
```
1. Prvo kreiramo *package.json*:
```
npm init
```

2. Zatim kreiramo **gulpfile.js** sa sledećim sadržajem

```
	//  Require Gulp into file and define the variable.
	var gulp = require('gulp');
	// 'hello' task definition.
	gulp.task('hello', function() {
	     console.log('Hello World!');
	});
```

3. Pomoću `git-bash` programa zatim instaliramo `gulp` lokalno u projekat pomoću sledeće komande
```
npm install gulp
npm link gulp </-- U slucaju da izbaci error(> npm ERR ! Invalid tag name "gulp":), moramo ga linkovati na globalnu instalaciju
```

Pokrenuti *hello* gulp task koji smo definisali unutar **gulpfile.js**
```
gulp hello
```

###### Ako je instalacija prosla uspešno klonirati *'mci-starter'* lokalno i instalirati ga gore korišćenim koracima.
###### Unutar projekta trenutno samo postoji 'default', koji radi `compile` scss fajlova u CSS i spaja naše JS fajlove koji se nalaze unutar JS foldera. 'default' task se pokreće sa komandom:
```
gulp
```







