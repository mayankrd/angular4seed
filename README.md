# Angular4seed

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.2.0.

## Pre-req
https://coursetro.com/posts/code/55/How-to-Install-an-Angular-4-App

## Steps for getting an Angular 4 app running from scratch (The LONG way)

###### 1. Create a new Angular 4 project using Angular CLI:
 `ng new angular4seed`
###### 2. Open project folder:
 `cd angular4seed`
###### 3. Run the app:
 `ng serve`
###### 4. Open app folder:
 `cd angular4seed/src/app`
###### 5. Adding a new component named 'task':
 `ng g c task`
###### 6. Navigating to the 'task' component. 
  ######    Add a constant array of routes in 'app.module':
  `const appRoutes: Routes = [
    { path: '', component: TaskComponent },
    { path: 'task', component: TaskComponent }
  ];`
  ######    Add an entry to the imports array:
  `RouterModule.forRoot(
        appRoutes,
        { enableTracing: true } 
        )`
###### 7. Add Router Outlet. Replace `templateUrl` to `template` with value `<router-outlet></router-outlet>`
  `@Component({
    selector: 'app-root',
    template: `<router-outlet></router-outlet>`,
    styleUrls: ['./app.component.css']
  })`
###### 8. Browse to `localhost:4200/task` or `localhost:4200/task`    

## Steps for getting an Angular 4 app running (The SHORT way :P)

   `git clone https://github.com/mayankrd/angular4seed.git`
   `cd angular4seed`
   `npm install`
   `ng serve`

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
