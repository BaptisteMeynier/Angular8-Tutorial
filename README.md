# Angular 8 Tutorial

# MyProjectName

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.2.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).


## Commands
Install angular cli component:  
npm install -g @angular/cli  

Be carreful when you use the command ng serve you can obtain the following error:  
```ERROR in ./src/polyfills.ts
  Module not found: Error: Can't resolve 'core-js/es6/reflect' in 'C:\Users\meynier\data\git\angular\Angular8-Tutorial\src'
  ERROR in ./src/polyfills.ts
  Module not found: Error: Can't resolve 'core-js/es7/reflect' in 'C:\Users\meynier\data\git\angular\Angular8-Tutorial\src'
  ** Angular Live Development Server is listening on localhost:4200, open your browser on http://localhost:4200/ **
  i ｢wdm｣: Failed to compile.
  i ｢wdm｣: Compiling...
```
To correct you just have to change file src/polyfills.ts  
```
import 'core-js/es6/reflect';  
import 'core-js/es7/reflect';  
```
to  
```
import 'core-js/es/reflect';  
import 'core-js/es/reflect';  
```

Launch local server :  
ng serve --open  
