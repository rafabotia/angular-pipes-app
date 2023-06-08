# PipesApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 14.2.11.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

## Instalar PrimeNg

A fecha de hoy junio 2023 es compatible con angular v14 y node 16
Instalar node 16: node-v16.15.1-x64
Instalar angular 14: npm install -g @angular/cli@14
También animaciones de angular: npm install @angular/animations --save

Para usar primeNg sin pagar es necesario instalar una versión NO LTS, o saldrá una banda roja arriba indicando:
You are using an LTS version of PrimeNG with an invalid license, you may either switch back to a non-LTS version or purchase a license at PrimeStore.

Como usamos angular 14, instalamos primeng v14:
npm i primeng@14 --save
npm install primeicons --save

en package.json se verá así:
{
...
  "primeicons": "^6.0.1",
  "primeng": "^14.2.3",
...
}

En angular.json:
      "architect": {
        "build": {
	    ....
	    ....
            "styles": [
              "src/styles.css",
              "node_modules/primeicons/primeicons.css",
              "node_modules/primeng/resources/themes/lara-light-indigo/theme.css",
              "node_modules/primeng/resources/primeng.min.css"
            ],

