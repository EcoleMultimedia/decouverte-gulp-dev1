# Découverte de Gulp

## Classe de DEV1 (promotion 2016)

Ce projet permet de mettre en pratique l'outil *Gulp* pour répondre à des problématiques souvent rencontrées en développement front-end en automatisant des tâches répétitives (compilation, concaténation, minification, ...)

# Installation

Cloner ce projet : `git clone git@github.com:jmpp/decouverte-gulp-dev1.git`

Récupérer les dépendences développeur : `npm install -d`

# Démarrage

Pour lancer un serveur local : `gulp` (équivaut à `gulp default`)

... et c'est tout ! Vous pouvez ensuite modifier à votre aise les sources (scripts et styles), gulp relancera les tâches nécessaires en un clin d'oeil.

## Tâches spécifiques

`gulp process-scripts` : S'occupe de concaténer et minifier les fichiers *.js* afin de produire `dist/app.js` et `dist/app.min.js`

`gulp process-styles` : S'occupe de builder les fichiers *.scss* avec SASS pour produire `dist/app.css` et `dist/app.min.css` (avec les [sourcemaps](https://medium.com/@toolmantim/getting-started-with-css-sourcemaps-and-in-browser-sass-editing-b4daab987fb0))

`gulp lint-scripts` : Permet de générer dans la console un petit rapport d'erreurs et/ou d'incohérences rencontrées sur les fichiers *.js* 

`gulp watch` : Surveille les modifications effectuées sur les fichiers *.js* et *.scss* et relance le cas échéant les tâches `process-scripts`, `lint-scripts` et `process-styles`
