JOSE VICENTE TEJERO CALDERERA	

05/10/2020

RESUMEN 
Exercise 1: Creating a Deploy Package Using webpack

Task 1: Install and configure Babel and webpack
He seguido los pasos indicados, crear package.json, instalar  npm install babel-core babel-loader babel-preset-es2015 webpack --save-dev
Crear webpack.config.js y 


DIFICULTAD: 
En la tarea 2, me da fallo al ejecutar:     npm run webpack

El log da el siguiente mensaje:
verbose cli [
1 verbose cli   'C:\\Program Files\\nodejs\\node.exe',
1 verbose cli   'C:\\Program Files\\nodejs\\node_modules\\npm\\bin\\npm-cli.js',
1 verbose cli   'run',
1 verbose cli   'webpack'
1 verbose cli ]
2 info using npm@6.14.8
3 info using node@v14.13.0
4 verbose stack Error: missing script: webpack
4 verbose stack     at run (C:\Program Files\nodejs\node_modules\npm\lib\run-script.js:155:19)
4 verbose stack     at C:\Program Files\nodejs\node_modules\npm\lib\run-script.js:63:5
4 verbose stack     at C:\Program Files\nodejs\node_modules\npm\node_modules\read-package-json\read-json.js:116:5
4 verbose stack     at C:\Program Files\nodejs\node_modules\npm\node_modules\read-package-json\read-json.js:436:5
4 verbose stack     at checkBinReferences_ (C:\Program Files\nodejs\node_modules\npm\node_modules\read-package-json\read-json.js:391:45)
4 verbose stack     at final (C:\Program Files\nodejs\node_modules\npm\node_modules\read-package-json\read-json.js:434:3)
4 verbose stack     at then (C:\Program Files\nodejs\node_modules\npm\node_modules\read-package-json\read-json.js:161:5)
4 verbose stack     at ReadFileContext.<anonymous> (C:\Program Files\nodejs\node_modules\npm\node_modules\read-package-json\read-json.js:350:20)
4 verbose stack     at ReadFileContext.callback (C:\Program Files\nodejs\node_modules\npm\node_modules\graceful-fs\graceful-fs.js:123:16)
4 verbose stack     at FSReqCallback.readFileAfterOpen [as oncomplete] (fs.js:265:13)
5 verbose cwd C:\aa\20480C\Allfiles\Mod15\Labfiles\Starter\ContosoConf
6 verbose Windows_NT 10.0.18363
7 verbose argv "C:\\Program Files\\nodejs\\node.exe" "C:\\Program Files\\nodejs\\node_modules\\npm\\bin\\npm-cli.js" "run" "webpack"
8 verbose node v14.13.0
9 verbose npm  v6.14.8
10 error missing script: webpack
11 verbose exit [ 1, true ]
