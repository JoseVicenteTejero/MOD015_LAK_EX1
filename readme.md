JOSE VICENTE TEJERO CALDERERA	

05/10/2020

RESUMEN 
Exercise 1: Creating a Deploy Package Using webpack

Task 1: Install and configure Babel and webpack
He seguido los pasos indicados, crear package.json, instalar  npm install babel-core babel-loader babel-preset-es2015 webpack --save-dev
Crear webpack.config.js y 


DIFICULTAD:  Hubo varios problemas pero ya están resueltos.
En la tarea 2, me da fallo al ejecutar:     npm run webpack
Añado en package.json lo siguiente:
"scripts": {
    "webpack": "webpack"
  }
 Ahora sí ejecuta npm run webpack pero da el siguiente error:
 
Error: Cannot find module 'webpack-cli'
Require stack:
- C:\aa\20480C\Allfiles\Mod15\Labfiles\Starter\ContosoConf\node_modules\webpack\bin\webpack.js
    at Function.Module._resolveFilename (internal/modules/cjs/loader.js:902:15)
    at Function.Module._load (internal/modules/cjs/loader.js:747:27)
    at Module.require (internal/modules/cjs/loader.js:974:19)
    at require (internal/modules/cjs/helpers.js:88:18)
    at C:\aa\20480C\Allfiles\Mod15\Labfiles\Starter\ContosoConf\node_modules\webpack\bin\webpack.js:143:5
    at processTicksAndRejections (internal/process/task_queues.js:93:5) {
  code: 'MODULE_NOT_FOUND',
  requireStack: [
    'C:\\aa\\20480C\\Allfiles\\Mod15\\Labfiles\\Starter\\ContosoConf\\node_modules\\webpack\\bin\\webpack.js'
  ]
}
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! @ webpack: `webpack`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the @ webpack script.

Instalamos C:\aa\20480C\Allfiles\Mod15\Labfiles\Starter\ContosoConf>npm install babel-loader@7
y volvemos a ejecutar: 
C:\aa\20480C\Allfiles\Mod15\Labfiles\Starter\ContosoConf>npm run webpack

> @ webpack C:\aa\20480C\Allfiles\Mod15\Labfiles\Starter\ContosoConf
> webpack

Hash: 191adb6fbae8ab741415
Version: webpack 4.44.2
Time: 3587ms
Built at: 05/10/2020 17:12:37
                      Asset      Size  Chunks                   Chunk Names
         feedback.bundle.js  3.55 KiB       0  [emitted]        feedback
     feedback.bundle.js.map  59.1 KiB       0  [emitted] [dev]  feedback
             live.bundle.js  3.52 KiB       1  [emitted]        live
         live.bundle.js.map  48.4 KiB       1  [emitted] [dev]  live
         location.bundle.js  1.82 KiB       2  [emitted]        location
     location.bundle.js.map  56.5 KiB       2  [emitted] [dev]  location
    locationVenue.bundle.js  1.24 KiB       3  [emitted]        locationVenue
locationVenue.bundle.js.map  29.9 KiB       3  [emitted] [dev]  locationVenue
          offline.bundle.js   1.4 KiB       4  [emitted]        offline
      offline.bundle.js.map  30.4 KiB       4  [emitted] [dev]  offline
         register.bundle.js  1.42 KiB       5  [emitted]        register
     register.bundle.js.map  30.7 KiB       5  [emitted] [dev]  register
         schedule.bundle.js  7.25 KiB       6  [emitted]        schedule
     schedule.bundle.js.map   141 KiB       6  [emitted] [dev]  schedule
     speakerBadge.bundle.js  5.43 KiB       7  [emitted]        speakerBadge
 speakerBadge.bundle.js.map   104 KiB       7  [emitted] [dev]  speakerBadge
            video.bundle.js  1.91 KiB       8  [emitted]        video
        video.bundle.js.map  56.2 KiB       8  [emitted] [dev]  video
Entrypoint video = video.bundle.js video.bundle.js.map
Entrypoint feedback = feedback.bundle.js feedback.bundle.js.map
Entrypoint live = live.bundle.js live.bundle.js.map
Entrypoint location = location.bundle.js location.bundle.js.map
Entrypoint locationVenue = locationVenue.bundle.js locationVenue.bundle.js.map
Entrypoint register = register.bundle.js register.bundle.js.map
Entrypoint schedule = schedule.bundle.js schedule.bundle.js.map
Entrypoint speakerBadge = speakerBadge.bundle.js speakerBadge.bundle.js.map
Entrypoint offline = offline.bundle.js offline.bundle.js.map
 [0] ./scripts/datetime.js 24.3 KiB {6} {8} [built]
 [1] ./scripts/pages/video.js 24.5 KiB {8} [built]
 [2] ./scripts/pages/feedback.js 24.2 KiB {0} [built]
 [3] ./scripts/StarRatingView.js 27.7 KiB {0} [built]
 [4] ./scripts/pages/live.js 23.7 KiB {1} [built]
 [5] ./scripts/LivePage.js 18 KiB {1} [built]
 [6] ./scripts/pages/location.js 24.7 KiB {2} [built]
 [7] ./scripts/geometry.js 24.2 KiB {2} [built]
 [8] ./scripts/pages/location-venue.js 24 KiB {3} [built]
 [9] ./scripts/pages/register.js 24.7 KiB {5} [built]
[10] ./scripts/pages/schedule.js 23.8 KiB {6} [built]
[11] ./scripts/ScheduleList.js 14.8 KiB {6} [built]
[14] ./scripts/LocalStarStorage.js 26.2 KiB {6} [built]
[15] ./scripts/pages/speaker-badge.js 23.6 KiB {7} [built]
[19] ./scripts/offline.js 24.3 KiB {4} [built]
    + 5 hidden modules

C:\aa\20480C\Allfiles\Mod15\Labfiles\Starter\ContosoConf>
