---
created: 2024-03-03
modified: 2024-03-03
tags:
  - framework
---

## Description
[[Angular]] is a [[TypeScript]] framework. As a platform, [[Angular]] includes: 
- A component-based framework for building scalable web applications
- A collection of well-integrated libraries that cover a wide variety of features, including routing, forms management, client-server communication, and more
- A suite of developer tools to help you develop, build, test, and update your code

learn more here: https://angular.io/guide/what-is-angular

## Starting a new [[Angular]] Project
### Installing the [[Angular]] [[../../3RESOURCES/DEFINITIONS/CLI]]
- The [[Angular]] [[../../3RESOURCES/DEFINITIONS/CLI]] is the command line interface used to create an application that already works, right out of the box. 
- To install [[Angular]] [[../../3RESOURCES/DEFINITIONS/CLI]] globally, type the following at the prompt in [[powershell]], no need to be in any particular directory
```bash
npm install -g @angular/cli@12.2.6
```
- **Note: find the latest version of [Angular](Angular.md) [CLI](../../3RESOURCES/DEFINITIONS/CLI.md) [here](https://www.npmjs.com/package/@angular/cli), along with all other packages installed using the npm install command**
- This will make the command line tool for creating Angular applications. To learn more about the various commands that this CLI provides, type at the prompt:
```bash
ng help
```



### Generating and Serving an [[Angular]] Project using [[Angular]] [[../../3RESOURCES/DEFINITIONS/CLI]]
- At a location in your C: drive, create a folder named *Angular* and move into that folder within [[powershell]]
	- Should look something like this: 
	- ![[Pasted image 20210917154857.png]]
		- **Note: make sure you are using "Run as Administrator"**
- Then, type the following at the prompt to create a new Angular application named as you desire: 
```bash
ng new <my program name here> --style=scss
```
- This should create a new folder within your *Angular* folder and create the [[Angular]] application within that folder 
	- **Note: a git repo is already setup within that folder, to verify, navigate to it and type "git status". To set up git, go to the [[Git]] page. This is not covered here**
- Move to your project folder and type the following at the prompt: 
```bash
ng serve --open 
```
- This will compile the project and then open a tab in your default browser at the address [http://localhost:4200](http://localhost:4200/).
- You can now set up an online [[Git]] repository and synchronize your project to the online repository. Make sure that the online [[Git]] repository is a private repository. 
### Getting started with [Angular Material](Angular%20Material.md)
This guide explains how to set up your Angular project to begin using Angular Material. It includes information on prerequisites, installing Angular Material, and optionally displaying a sample Material component in your application to verify your setup.

_Angular Resources_

If you are new to Angular or getting started with a new Angular application, see [Angular's full Getting Started Guide](https://angular.io/start) and [Setting up your environment](https://angular.io/guide/setup-local).

For existing applications, follow the steps below to begin using Angular Material.

#### Install Angular Material
Use the Angular CLI's installation [schematic](https://material.angular.io/guide/schematics) to set up your Angular Material project by running the following command:
```
ng add @angular/material 
```

The ``` ng add ``` command will install Angular Material, the [[CDK)](https://material.angular.io/cdk/categories|Component Dev Kit (CDK)]], [Angular Animations](https://angular.io/guide/animations) and ask you the following questions to determine which features to include:
1.  Choose a prebuilt theme name, or "custom" for a custom theme: You can choose from [[https://material.angular.io/guide/theming#using-a-pre-built-theme]] or set up an extensible [[https://material.angular.io/guide/theming#defining-a-theme]].
2.  Set up global Angular Material typography styles: Whether to apply the global [typography](https://material.angular.io/guide/typography) styles to your application.
3.  Set up browser animations for Angular Material:

Importing the [`BrowserAnimationsModule`](https://angular.io/api/platform-browser/animations/BrowserAnimationsModule) into your application enables Angular's [animation system](https://angular.io/guide/animations). Declining this will disable most of Angular Material's animations.

The `ng add` command will additionally perform the following actions:
-   Add project dependencies to `package.json`
-   Add the Roboto font to your `index.html`
-   Add the Material Design icon font to your `index.html`
-   Add a few global CSS styles to:
    -   Remove margins from `body`
    -   Set `height: 100%` on `html` and `body`
    -   Set Roboto as the default application font

You're done! Angular Material is now configured to be used in your application.
#### (test) Display a Component
Let's display a slider component in your app and verify that everything works.

You need to import the `MatSliderModule` that you want to display by adding the following lines to your `app.module.ts` file.

```ts
import { MatSliderModule } from '@angular/material/slider';

@NgModule ({
  imports: [
    MatSliderModule,
  ]
})
class AppModule {}
```

Add the `<mat-slider>` tag to the `app.component.html` like so:

```html
<mat-slider min="1" max="100" step="1" value="50"></mat-slider>
```

Run your local dev server:

```bash
ng serve
```

Then point your browser to [http://localhost:4200](http://localhost:4200/)

You should see the Material slider component on the page.

In addition to the installation schematic, Angular Material comes with [several other schematics](https://material.angular.io/guide/schematics) (like nav, table, address-form, etc.) that can be used to easily generate pre-built components in your application.


## Working with [[Angular]] Components
### Creating a New Component 
#### From Scratch 
```bash
ng generate component <component-name>
```
- This will generate a folder in your project folder named `component-name`
- Inside this folder will be: 
	- `component-name.component.html`
		- a template file 
	- `component-name.component.scss`
		- or another style format (.css for example)
	- `component-name.component.spec.ts`
		- a testing specification file
		- you can usually just delete this
	- `component-name.component.ts`
		- your component file

#### From a Schematic

# to be added 
## routing 
- Routing in angular 
- add html routerLink to <a></a> stuff
	- This is an [[HTML a Tag]]
- This will trigger a router link when you perform an action. 

EX: 
```html
	<a mat-list-item routerLink="/home">Home</a>

```

- edit app-routing.module.ts
- add the following code: 
```ts
const routes: Routes = [
]
```
- direct the routes with the following syntax within the routes array

```ts
{path:'home', component:homeComponent}
```
- This component will get loaded in the <router-outlet></router-outlet> HTML tag if the following url is followed: http://localhost:4200/home
- **Note: make sure you have a home component before you do this**
## API calling in angular
API in TS: https://youtu.be/rdLJNGZvlAA

## Data binding in [[Angular]]
```html
<li>{{hero.name}}</li> 
<app-hero-detail [hero]="selectedHero"></app-hero-detail> 
<li (click)="selectHero(hero)"></li>
```

-   The `{{hero.name}}` [_interpolation_](https://angular.io/guide/interpolation) displays the component's `hero.name` property value within the `<li>` element.
    
-   The `[hero]` [_property binding_](https://angular.io/guide/property-binding) passes the value of `selectedHero` from the parent `HeroListComponent` to the `hero` property of the child `HeroDetailComponent`.
    
-   The `(click)` [[https://angular.io/guide/user-input#binding-to-user-input-events]] calls the component's `selectHero` method when the user clicks a hero's name.

### Two-way binding 
```html
<input type="text" id="hero-name" [([ngModel)]="hero.name">
```
- In two-way binding, a data property value flows to the input box from the component as with property binding. The user's changes also flow back to the component, resetting the property to the latest value, as with event binding.


## Pipes in [[Angular]]
### Pipes

Angular pipes let you declare display-value transformations in your template HTML. A class with the @[Pipe](https://angular.io/api/core/Pipe) decorator defines a function that transforms input values to output values for display in a view.

Angular defines various pipes, such as the [date](https://angular.io/api/common/DatePipe) pipe and [currency](https://angular.io/api/common/CurrencyPipe) pipe; for a complete list, see the [Pipes API list](https://angular.io/api?type=pipe). You can also define new pipes.

To specify a value transformation in an HTML template, use the [[|)](https://angular.io/guide/pipes|pipe operator (|)]].

`{{interpolated_value | pipe_name}}`

You can chain pipes, sending the output of one pipe function to be transformed by another pipe function. A pipe can also take arguments that control how it performs its transformation. For example, you can pass the desired format to the [date](https://angular.io/api/common/DatePipe) pipe.
## Template driven forms 
Example form input in angular (template driven)
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-template-favorite-color',
  template: `
    Favorite Color: <input type="text" [(ngModel)]="favoriteColor">
  `
})
export class FavoriteColorComponent {
  favoriteColor = '';
}

```