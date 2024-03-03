---
created: 2021-09-13
modified: 2024-03-03
tags:
  - class-notes
---


https://www.coursera.org/learn/angular/home/welcome

## Notes: 
### Week 1
#### Full stack Web Development: The Big Picture: Objectives and Outcomes

This lesson gives you a big picture view of the Full Stack Web Development. The lecture gives you an overview of full stack web development. At the end of this lesson, you will be able to:

-   Understand what is meant by full stack in the context of web development
-   Distinguish between front-end, back-end and full stack web development
-   Understand the position of this course in the context of this specialization

#### What is Full-Stack Web Development?
Front end: delivering content to user: 
	HTML, CSS and Javascript
Back end/ server-side
	Various tech and approaches
	PHP, Java, ASP.NET, Ruby, Python

Three Tier Architecture: 
	Presentation Layer
		concerned with UI 
		HTML, CSS, JS
	Business Logic layer
		concerned with data validation, dynamic content processing
		Ruby, python, java, C++, PHP
	Data Access layer
		Data persistence, data access through an API
		DBMS
	This makes up a full stack 
	
These three tiers are being increasingly encompassed by just Javascript 
![[ATTACHMENTS/Pasted image 20210910145433.png]]

Angular -> NodeJS -> JSON/MongoDB	
#### Setting up Your Development Environment: Git and Node
##### Objectives
At the end of this lesson you should have set up Git and Node.js on your computer. At the end of this lesson, you will be able to:

-   Set up a Git repository and perform basic Git operations
-   Set up and use online Git repositories
-   Use Node-based modules to perform basic operations.

##### Setting up your Development Environment
 Software Requirements

1.  **Text editor of your choice**: Any text editor that you are already familiar with can be used for editing the project files. I will be using Visual Studio Code ([https://code.visualstudio.com/](https://code.visualstudio.com/)) as the editor of choice in this specialization. You may also consider other editors such as Brackets ([http://brackets.io/](http://brackets.io/)), Sublime Text ([http://www.sublimetext.com/)](http://www.sublimetext.com/)), or Atom ([https://atom.io/](https://atom.io/)).
    
2.  **Browser of your choice**: You may use your preferred browser. I will be using Chrome as the browser in all the exercises. All the exercises and assignments in this course have been tested using Chrome v. 46. Please note that not all browsers may support all the HTML5 features to the same extent. You might encounter problems when using other browsers. I strongly urge you to use the latest Chrome browser for the exercises and assignments in this course so that any problems are minimized.
    
3.  **Command line shell**: Familiarity with the command-line shell will be essential for the exercises. In Windows a cmd window or power shell with admin privileges would be needed. On a Mac or in Linux, a terminal window can be used. Please get familiar with the "[sudo](http://www.tutorialspoint.com/unix_commands/sudo.htm)" command in OS X and Linux.
    
4.  **Files required for the exercises**: We will provide additional starter files for the exercises wherever needed. Links to download the files will be provided inline in the **exercise instructions** that follow each exercise video. Please download the files provided there, if any, before beginning the exercise. The links are also available through the **Additional Resources** of the specific lesson.
    

Note: Please remember to retain the folders and all the files that you create in the exercises. Further exercises will build upon the files that you create in the preceding exercises. DO NOT DELETE the files at the end of the exercises, unless otherwise instructed. You may wish to set up your exercise folder as a Git repository and commit the files to the repository at the end of each exercise. Brief instructions on using Git are available later in this lesson.

##### Setting up Git
Version control software

go to git-scm.com

[[git book]]

![[ATTACHMENTS/Pasted image 20210910151406.png]]

Now to configure global identity parameters
username and email address
use command: git config --global user.name "username"
	git config --global user.email email
use git config --list to list all config settings 
	
##### Basic Git commands
git init
	initializes the current folder as a git repository
	This is the master branch for the git
git status
	current status of the folder
	
git add (files/folders)
	adds files and folders to the staging area
git commit 
	commits the changes to the git repository

git log - oneline
	see a brief log of commits
git checkout (commit)(file)
	checkout the file from an older commit

---


##### Online [[Git]] Repositories 
###### Objectives and Outcomes
In this exercise you will learn about how to set up and use an online Git repository and synchronize your local Git repository with your online repository. At the end of this exercise, you will be able to:
-   Set up the online repository as a remote repository for your local Git repository
-   Push your commits to the online repository
-   Clone an online Git repository to your computer

###### Setting up an Online Git repository
-   Sign up for an account either at Bitbucket ([https://bitbucket.org](https://bitbucket.org/)) or GitHub ([https://github.com](https://github.com/)). Note that private repositories on GitHub requires a paid account, and is not available for free accounts.
-   set up repository named git-test

###### Set the local Git repository to set its remote origin
-   At the prompt, type the following to set up your local repository to link to your online Git repository:
![[ATTACHMENTS/Pasted image 20210915132405.png]]
must be in the repository, for example, mine is C:\Users\AlexaLo\OneDrive - Lam Research\Desktop\git-test


###### Pushing your commits to the online repository 
-   At the prompt, type the following to push the commits to the online repository:
-   ![[ATTACHMENTS/Pasted image 20210915132714.png]]

###### Cloning an online repository
-   To clone an online repository to your computer, type the following at the prompt
-   ![[ATTACHMENTS/Pasted image 20210915132851.png]]
###### Conclusions
In this exercise you have learned to set up an online Git repository, synchronize your local repository with the remote repository, and clone an online repository.
##### Setting up [[Node.js]] and [[NPM]]
**Note: Make sure you have installed Git on your machine before you install Node.js. Please complete the previous Git installation exercise before proceeding with this exercise.**

###### Objectives and Outcomes 
In this exercise, you will learn to set up the Node.js environment, a popular Javascript based server framework, and node package manager (NPM) on your machine. To learn more about NodeJS, you can visit [https://nodejs.org](https://nodejs.org/). For this course, you just need to install Node.js on your machine and make use of it for running some front-end tools. You will learn more about the server-side support using Node.js in a subsequent course. At the end of this exercise, you will be able to:

-   Complete the set up of Node.js and NPM on your machine
    
-   Verify that the installation was successful and your machine is ready for using Node.js and NPM.
###### Installing Node
-   To install Node on your machine, go to [https://nodejs.org](https://nodejs.org/) and click on the Download button. Depending on your computer's platform (Windows, MacOS or Linux), the appropriate installation package is downloaded.
-   As an example, on a Mac, you will see the following web page. Click on the Download button. Follow along the instructions to install Node on your machine. (Note: Now Node gives you the option of installing a mature and dependable LTS version and a more newer stable version. You should to install the LTS version. I will use this version in the course.)
-   ![[ATTACHMENTS/Pasted image 20210915134548.png]]

**Note: On Windows machines, you may need to configure your PATH environmental variable in case you forgot to turn on the add to PATH during the installation steps.**
###### Verifying the Node Installation
-   Open a terminal window on your machine. If you are using a Windows machine, open a cmd window or PowerShell window with **admin** privileges.
    
-   To ensure that your NodeJS setup is working correctly, type the following at the command prompt to check for the version of **Node** and **NPM**

![[ATTACHMENTS/Pasted image 20210915134721.png]]
![[ATTACHMENTS/Pasted image 20210915134749.png]]

##### Basics of [[Node.js]] and NPM 
###### Objectives and Outcomes 
In this exercise you will learn the basics of Node and NPM. At the end of this exercise, you will be able to:

-   Set up package.json file in the project folder for configuring your Node and NPM for this project
    
-   Install a NPM module and make use of it within your project


###### Initializing package.json
-   At the command prompt in your **git-test** folder, type
-   ![[ATTACHMENTS/Pasted image 20210915135406.png]]
-   Follow along the prompts and answer the questions as follows: accept the default values for most of the entries, except set the entry point to index.html
-   This should create a _package.json_ file in your **git-test** folder.
![[ATTACHMENTS/Pasted image 20210915135739.png]]


###### Installing an NPM Module
-   Install an NPM module, lite-server, that allows you to run a Node.js based development web server and serve up your project files. To do this, type the following at the prompt:
-   ![[ATTACHMENTS/Pasted image 20210915135841.png]]
-   -   You can check out more documentation on lite-server [here](https://github.com/johnpapa/lite-server).
    
-   Next, open package.json in your editor and modify it as shown below. Note the addition of two lines, line 7 and line 9.
```javascript
{
 	"name": "git-test",
 	"version": "1.0.0",
 	"description": "This is the Git and Node basic learning project",
 	"main": "index.html",
 	"scripts": {
 		"start": "npm run lite",
 		"test": "echo \"Error: no test specified\" && exit 1",
 		"lite": "lite-server"
 },
 	"repository": {
 		"type": "git",
		"url": "git+https://jogesh_k_muppala@bitbucket.org/jogesh_k_muppala/git-test.git"
 },
 	"author": "",
 	"license": "ISC",
 	"homepage": "https://bitbucket.org/jogesh_k_muppala/git-test#readme",
 	"devDependencies": {
 		"lite-server": "^2.2.2"
 }
}

```
-   Next, start the development server by typing the following at the prompt:
-   ![[ATTACHMENTS/Pasted image 20210915140441.png]]
-   This should open your _index.html_ page in your default browser.
    
-   If you now open the _index.html_ page in an editor and make changes and save, the browser should immediately refresh to reflect the changes.


###### Setting up .gitignore
-   Next, create a file in your project directory named _.gitignore_ (**Note**: the name starts with a period)Then, add the following to the .gitignore file
-   ![[ATTACHMENTS/Pasted image 20210915140653.png]]
-   Then do a git commit and push the changes to the online repository. You will note that the node_modules folder will not be added to the commit, and will not be uploaded to the repository
##### Setting up your development Environment: [[Git]] and [[Node.js]]: Additional Resources
###### Additional Resources ([[Git]])
-   Git site [http://git-scm.com](http://git-scm.com/).
    
-   [Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) chapter from Pro Git
    
-   [Git reference manual](https://git-scm.com/docs)
    
-   Quick reference guides: [GitHub Cheat Sheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf) (PDF) | [Visual Git Cheat Sheet](http://ndpsoftware.com/git-cheatsheet.html) (SVG | PNG)
    
-   [Atlassian comprehensive Git tutorial](https://www.atlassian.com/git/tutorials/)


###### Additional Resources ([[Node.js]] and [[NPM]])
-   [Nodejs.org](https://nodejs.org/)
    
-   [Npmjs.com](https://www.npmjs.com/)
    
-   [Node API Documentation](https://nodejs.org/api/)
    
-   [NPM Documentation](https://docs.npmjs.com/)
    
-   [lite-server](https://github.com/johnpapa/lite-server)
#### Introduction to Angular 
##### Introduction to [[Angular]]: Objectives and Outcomes
In this lesson you will be given a quick overview of JavaScript frameworks and then introduced to [[Angular]] in particular. We will learn some basics of [[Angular]] and how to configure an [[Angular]] application using the [[Angular]]-[[../../3RESOURCES/DEFINITIONS/CLI]], the command line tool. At the end of this lesson, you will be able to:

-   Get a basic overview of JavaScript frameworks
    
-   Understand the architecture of an [[Angular]] application
    
-   Scaffold out a starter [[Angular]] application using _angular-cli_, the command line tool
##### Front-end JavaScript Frameworks Overview 
What is a software library?
- a software library is a collection of implementations of behaviors that you repeatedly use within your applications.

Software library v. a software framework 
- A software framework is an abstraction in which the software provides such generic functionality and then provides you with the ability of customizing that functionality for implementing the solutions for your specific application.
- this is a different way of thinking about how you attempt to solve the problem as opposed to using a software library.
- [[Angular]] is a software framework 


##### Getting started with [[Angular]]
###### Objectives and Outcomes 
In this first [[Angular]] exercise, you will first install _angular-cli_, the command line tool for scaffolding Angular applications. You will then use the tool to scaffold out a basic [[Angular]] application. We will thereafter develop this application into a full-fledged Angular application in the process of doing the exercises in this course. At the end of this exercise you will be able to:

-   Install _angular-cli_
    
-   Scaffold out a basic Angular application

Installing _Angular-CLI_

From the [[Angular]]-[[../../3RESOURCES/DEFINITIONS/CLI]] documentation we learn that the [[Angular]] [[../../3RESOURCES/DEFINITIONS/CLI]] makes it easy to create an application that already works, right out of the box. It already follows the best practices suggested by the Angular community!

-   To install _angular-cli_ globally, type the following at the prompt:
-   ![[ATTACHMENTS/Pasted image 20210915154545.png]]

Use _sudo_ on a Mac and Linux

-   This will make the command line tool for creating Angular applications. To learn more about the various commands that this CLI provides, type at the prompt:
-   ![[ATTACHMENTS/Pasted image 20210915154655.png]]


###### Generating and Serving an Angular Project using Angular-CLI
-   At a convenient location on your computer, create a folder named _Angular_ and move into that folder.
    
-   Then type the following at the prompt to create a new Angular application named _conFusion_:
-   ![[ATTACHMENTS/Pasted image 20210915155645.png]]
-   This should create a new folder named _conFusion_ within your _Angular_ folder and create the Angular application in that folder.
    
-   Move to the conFusion folder and type the following at the prompt:
-   ![[ATTACHMENTS/Pasted image 20210915155701.png]]
-   Just like this baby
-   ![[ATTACHMENTS/Pasted image 20210915163954.png]]
-   This will compile the project and then open a tab in your default browser at the address [http://localhost:4200](http://localhost:4200/).
    
-   You can initialize your project to be a Git repository by typing the following commands at the prompt:
-   ![[ATTACHMENTS/Pasted image 20210915163747.png]]
-   **Note**: You will notice that this will reinitialize the Git repository and you will see the first commit with the message "initial commit" already in the repository.

-   Thereafter you can set up an online Git repository and synchronize your project to the online repository. Make sure that the online Git repository is a **_private_** repository.

##### Configuring your [[Angular]] application
###### Objectives and Outcomes
In this exercise we will set up our project to use Angular Material and Angular Flex Layout. We will then introduce our first Angular Material component into our application. At the end of this exercise you will be able to:

-   Configure your Angular project to use Angular Material and Flex Layout.
    
-   Start using Material components in your application.
###### Configure your Angular Project to use Angular Material 
-   To configure your project to use Angular material, type the following at the prompt to install Angular Material, Angular Animations and HammerJS:
```
	npm install @angular/material@6.4.7 --save
	npm install @angular/cdk@6.4.7 --save
	npm install --save @angular/animations@6.1.7
	npm install --save hammerjs@2.0.8
```
- go to https://www.npmjs.com/ for lists of latest package versions

###### Configure to use Material Design Icons
- Next, include the following into the head of the index.html to make use of material design icons: 

```
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">

```


###### Configure your Angular Project to use Flex Layout
- Next, install Angular Flex Layout as follows: 

```
npm install --save @angular/flex-layout@12.0.0-beta.35
```


###### Updating AppModule
-   Then, you need to import the Angular Animations Module, Angular Material Toolbar Module, Flex Layout Module and hammerjs into your root module (src/app/app.module.ts) as follows:

```
. . . 

  

import { BrowserAnimationsModule } from '@angular/platform-browser/animations';

import { MatToolbarModule } from '@angular/material/toolbar'; 

import { FlexLayoutModule } from '@angular/flex-layout';

  

. . . 

  

import 'hammerjs';

  

@NgModule({

 . . . 

 imports: [ 

 . . .,

 BrowserAnimationsModule,

 MatToolbarModule,

 FlexLayoutModule

 ], 

 . . . 

}) 

  

. . .
```

###### Adding styles
- add the following styles to styles.scss file: 

```
@import '~@angular/material/prebuilt-themes/deeppurple-amber.css';

  

// some basic resets 

  

body { 

 padding: 0; 

 margin: 0; 

 font-family: Roboto, sans-serif; 

}
```

-   This will add a built-in Material theme to our application.
    
-   Do a Git commit with the message "Configuring Angular"

Warning: must install @angular/cdk to run stuff these days
##### Introduction to Angular: Additional Resources
###### Angular Resources
-   [Angular.io](https://angular.io/)    
-   [Angular CLI](https://cli.angular.io/)    
-   [Angular Material](https://material.angular.io/)    
-   [Angular Material Toolbar](https://material.angular.io/components/toolbar/overview)    
-   [Angular Flex Layout](https://github.com/angular/flex-layout)    
-   [Angular Flex Layout Documentation](https://github.com/angular/flex-layout/wiki/API-Documentation)

###### Typescript 
-   [Typescript](http://www.typescriptlang.org/index.html)
-   [Typescript Tutorial](http://www.typescriptlang.org/docs/tutorial.html)    
-   [Typescript: Migrating from JavaScript](http://www.typescriptlang.org/docs/handbook/migrating-from-javascript.html)

###### Definitions 
-   [Framework](https://en.wikipedia.org/wiki/Software_framework)    
-   [Hollywood Principle](https://en.wikipedia.org/wiki/Hollywood_principle)
-   [Inversion of Control](https://en.wikipedia.org/wiki/Inversion_of_control)
-   [Imperative vs Declarative Programming](https://netguru.co/blog/imperative-vs-declarative)
-   [Imperative vs Declarative](http://latentflip.com/imperative-vs-declarative/)

###### Blog Articles 
-   [[https://hackernoon.com/5-best-javascript-frameworks-in-2017-7a63b3870282#.tt1k09l1d]]
-   [[https://medium.com/javascript-scene/top-javascript-frameworks-topics-to-learn-in-2017-700a397b711#.pe809bf0u]]
-   [Declarative vs. Imperative Programming for the Web](http://codenugget.co/2015/03/05/declarative-vs-imperative-programming-web.html)
-   [[https://medium.com/@ladyleet/using-angular-material2-components-in-your-angular-2-project-intro-custom-styles-buttons-d2178e4b45c5#.y8cz8yk0r]]
#### Angular Components
##### Angular Components: Objectives and Outcomes
In this lesson you will learn about Angular components and how we construct an Angular component and design its views. At the end of this lesson you will be able to:

-   Use Angular-CLI to scaffold out the barebones of an Angular component
    
-   Construct the Angular component code and the template for your component


##### Angular Components part 1
###### Objectives and Outcomes
In this exercise you will add the first component to your Angular application and update its template. At the end of this exercise you will be able to:

-   Add components to your Angular application
    
-   Update the templates of your component.


###### Adding a Menu component
-   First, download the images.zip file provided above and then unzip the file. Move the resulting _images_ folder containing some PNG files to the Angular project's _src/assets_ folder. These image files will be useful for our exercises.
    
-   Next, use the CLI's _ng generate_ command to generate a new component named menu as follows:

```
ng generate component menu
```

-   This will create the necessary files for the menu component in a folder named _menu_, and also import this component into _app.module.ts_.
    
-   Next, open app.component.html file and add the following after the toolbar:

```
<app-menu></app-menu>
```

###### Creating the Menu
-   Next, create a folder named _shared_ under the _src/app_ folder. To this folder, add a file named dish.ts with the following code:

```
export class Dish {

 id: string;

 name: string;

 image: string;

 category: string;

 featured: boolean;

 label: string;

 price: string;

 description: string;

}
```

-   Update menu.component.ts as follows to add in the data for four menu items:

```
. . .

import { Dish } from '../shared/dish';

. . .

  

export class MenuComponent implements OnInit {

  

 dishes: Dish[] = [

 {

 id: '0',

 name: 'Uthappizza',

 image: '/assets/images/uthappizza.png',

 category: 'mains',

 featured: true,

 label: 'Hot',

 price: '4.99',

 // tslint:disable-next-line:max-line-length

 description: 'A unique combination of Indian Uthappam (pancake) and Italian pizza, topped with Cerignola olives, ripe vine cherry tomatoes, Vidalia onion, Guntur chillies and Buffalo Paneer.'

 },

 {

 id: '1',

 name: 'Zucchipakoda',

 image: '/assets/images/zucchipakoda.png',

 category: 'appetizer',

 featured: false,

 label: '',

 price: '1.99',

 description: 'Deep fried Zucchini coated with mildly spiced Chickpea flour batter accompanied with a sweet-tangy tamarind sauce'

 },

 {

 id: '2',

 name: 'Vadonut',

 image: '/assets/images/vadonut.png',

 category: 'appetizer',

 featured: false,

 label: 'New',

 price: '1.99',

 description: 'A quintessential ConFusion experience, is it a vada or is it a donut?'

 },

 {

 id: '3',

 name: 'ElaiCheese Cake',

 image: '/assets/images/elaicheesecake.png',

 category: 'dessert',

 featured: false,

 label: '',

 price: '2.99',

 description: 'A delectable, semi-sweet New York Style Cheese Cake, with Graham cracker crust and spiced with Indian cardamoms'

 }

 ];

. . .

}
```

-   Next, update the menu.component.html template as follows:

```
<div class="container"

 fxLayout="column"

 fxLayoutGap="10px">

  

 <mat-list fxFlex>

 <mat-list-item *ngFor="let dish of dishes">

 <img matListAvatar src={{dish.image}} alt={{dish.name}}>

 <h1 matLine> {{dish.name}} </h1>

 <p matLine>

 <span> {{dish.description}} </span>

 </p>

 </mat-list-item>

 </mat-list>

  

</div>
```

-   Next, open _app.module.ts_ and update it as follows:

```
. . .

  

import { MatListModule } from '@angular/material/list';

  

. . .

  

 imports: [

 . . .,

 MatListModule,

 . . .

 ],

  

. . .
```

-   Add the following CSS class to styles.scss file:

```
.container {

 margin: 20px;

 display:flex;

}
```



##### Angular Components part 2 
###### Objectives and Outcomes 
In this exercise we will continue modifying the component template from the previous exercise. Instead of a list, we will use a grid list Angular material component to display the menu in a different way. Also we will use the Card component to display the details of a selected dish. At the end of this exercise you will be able to:

-   Make use of the Angular material grid list component to display a list of items.
    
-   Use the material Card component to display detailed information.
    
-   Use a built-in Angular pipe to turn a word into uppercase in the template.


###### Updating the Menu Template
-   Open _menu.component.html_ and update its content as follows:

```html
<div class="container"

 fxLayout="column"

 fxLayoutGap="10px">

  

 <div fxFlex>

 <div>

 <h3>Menu</h3>

 <hr>

 </div>

 </div>

  

 <div fxFlex>

 <mat-grid-list cols="2" rowHeight="200px">

 <mat-grid-tile *ngFor="let dish of dishes">

 <img height="200px" src={{dish.image}} alt={{dish.name}}>

 <mat-grid-tile-footer>

 <h1>{{dish.name | uppercase}}</h1>

 </mat-grid-tile-footer>

 </mat-grid-tile>

 </mat-grid-list>

 </div>

  

</div>
```

-   Here we are using the Grid list Angular material component to display the information.
    
-   Open _app.module.ts_ and update it as follows:

```
. . .

  

import { MatGridListModule } from '@angular/material/grid-list';

import { MatCardModule } from '@angular/material/card';

import { MatButtonModule } from '@angular/material/button';

  

. . .

  

 imports: [

 . . .,

 MatGridListModule,

 MatCardModule,

 MatButtonModule,

 . . .

 ],

  

. . .
```
-   Also, update the _menu.component.ts_ file as follows to move the details of the dishes into a constant, in preparation for introducing services in a future exercise:

```
 . . .

 const DISHES: Dish[] = [

 . . .

 ];

 . . .

 export class MenuComponent implements OnInit {

  

 dishes = DISHES;

  

 selectedDish = DISHES[0];

  

 . . .

 }
```


###### Add a card component
-   Update the menu.component.html template to display the details of a selected dish using the Material Card component as follows:

```
 <div fxFlex *ngIf="selectedDish">

 <mat-card>

 <mat-card-header>

 <mat-card-title>

 <h3>{{selectedDish.name | uppercase}}</h3>

 </mat-card-title>

 </mat-card-header>

 <img mat-card-image src={{selectedDish.image}} alt={{selectedDish.name}}>

 <mat-card-content>

 <p>{{selectedDish.description}}

 </p>

 </mat-card-content>

 <mat-card-actions>

 <button mat-button>LIKE</button>

 <button mat-button>SHARE</button>

 </mat-card-actions>

 </mat-card>

 </div>

```


##### Directives
- A component is a special kind of directive with a template associated
- Two other kinds: 
	- Structural and attribute 

- Structural directives 
	- Allows you to alter the layout by adding, removing and replacing elements in the DOM 
	- Common structural directives
		- NGIf
			- `<div *ngIf="selectedDish">...</div>`
			- remove the div from the [[DOM]] if the value turns out to be false 
		- NgFor
			- `<mat-list-item *ngFor="let dish of dishes">...<mat-list-item>`
		- NgSwitch


#### Peer Graded Assignment: Angular Components
###### Objectives and outcomes 
In this assignment, you will continue to work with the Angular application that you have been developing in the exercises. You will add a new component named **_dishdetail_** that will display the details of a selected dish. You will then design the template for the component using Angular material components. At the end of this assignment, you should have completed the following tasks:

-   Created a new dishdetail component and added it to your Angular application and included it into the template of the menu component.
    
-   Updated the template of the dishdetail component to display the details of the selected dish using an Angular card component.
    
-   Updated the template of the dishdetail component to display the list of comments about the dish using the Angular material list component.


###### Assignment Requirements 
This assignment requires you to complete the following tasks. Detailed instructions for each task are given below. The picture of the completed web page included below indicates the location within the web page that will be updated by the three tasks.


###### Task 1
In this task you will be adding a new **_dishdetail_** component to your Angular application and include the component into the menu component's template so that the details of a specific dish are displayed there:

-   Use Angular CLI to create a new component named **_dishdetail_**,
    
-   Replace the card showing the selected dish in menu component's template with the dishdetail component, and
    
-   Update the template of the dishdetail component with the following code:


### Week 2
#### Angular Services, Routing and Single Page Applications
In this week, you learn about data binding in Angular. You will learn how to design basic services. You will learn about Angular router and its use in designing single page applications. You will also learn about single page applications and use Angular Router to design single page applications.
#### Learning Objectives 
-   Describe the various ways that data binding is used in an Angular application
-   Create a service that enables the Angular application to encapsulate all data related operations
-   Develop an Angular router to enable navigating to various views in your Angular application
-   Develop a single page application using the Angular router support

#### Data Binding
##### Data Binding: Objectives and Outcomes
In this lesson you will learn about data binding and how data binding enables the flow of information between the component and its template. You will learn about interpolation, property attribute and event binding and the use of two-way data binding. At the end of this lesson you will be able to:
- Understand how the data flows between the component code and its template
- Understand how one-way and two-way data binding can be used to effect the flow of data 


##### Exercise: Data Binding 
###### Objectives and outcomes

In this exercise you will use your knowledge of data binding to update the Angular application to enable you to select any dish from the menu and show its details. At the end of this exercise you will be able to:

-   Leverage data binding for communication among components
    
-   Design a component to receive input from another component.
###### Refactoring the Code
-   First, create a new class named Comment in a file named comment.ts in the shared folder and include the following in it:

```js
export class Comment {
 rating: number;
 comment: string;
 author: string;
 date: string;
}
```

-   Then update the dish class to allow a dish to have an array of comments as follows:

```js
import { Comment } from './comment';

export class Dish {
 . . .
 comments: Comment[];
}
```

-   Then create a new file named dishes.ts in the shared folder to now export the JavaScript object array of dishes:

```js
import { Dish } from './dish';
  
export const DISHES: Dish[] = [
 	{
 		id: '0',
 		name: 'Uthappizza',
 		image: '/assets/images/uthappizza.png',
 		category: 'mains',
 		featured: true,
 		label: 'Hot',
 		price: '4.99',
 		// tslint:disable-next-line:max-line-length		description:'A unique combination of Indian Uthappam (pancake) and Italian pizza, topped with Cerignola olives, ripe vine cherry tomatoes, Vidalia onion, Guntur chillies and Buffalo Paneer.',
 comments: [
 {
 rating: 5,
 comment: 'Imagine all the eatables, living in conFusion!',
 author: 'John Lemon',
 date: '2012-10-16T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Sends anyone to heaven, I wish I could get my mother-in-law to eat it!',
 author: 'Paul McVites',
 date: '2014-09-05T17:57:28.556094Z'
 },
 {
 rating: 3,
 comment: 'Eat it, just eat it!',
 author: 'Michael Jaikishan',
 date: '2015-02-13T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Ultimate, Reaching for the stars!',
 author: 'Ringo Starry',
 date: '2013-12-02T17:57:28.556094Z'
 },
 {
 rating: 2,
 comment: 'It\'s your birthday, we\'re gonna party!',
 author: '25 Cent',
 date: '2011-12-02T17:57:28.556094Z'
 }
 ]
 },
 {
 id: '1',
 name: 'Zucchipakoda',
 image: '/assets/images/zucchipakoda.png',
 category: 'appetizer',
 featured: false,
 label: '',
 price: '1.99',
 description: 'Deep fried Zucchini coated with mildly spiced Chickpea flour batter accompanied with a sweet-tangy tamarind sauce',
 comments: [
 {
 rating: 5,
 comment: 'Imagine all the eatables, living in conFusion!',
 author: 'John Lemon',
 date: '2012-10-16T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Sends anyone to heaven, I wish I could get my mother-in-law to eat it!',
 author: 'Paul McVites',
 date: '2014-09-05T17:57:28.556094Z'
 },
 {
 rating: 3,
 comment: 'Eat it, just eat it!',
 author: 'Michael Jaikishan',
 date: '2015-02-13T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Ultimate, Reaching for the stars!',
 author: 'Ringo Starry',
 date: '2013-12-02T17:57:28.556094Z'
 },
 {
 rating: 2,
 comment: 'It\'s your birthday, we\'re gonna party!',
 author: '25 Cent',
 date: '2011-12-02T17:57:28.556094Z'
 }
 ]
 },
 {
 id: '2',
 name: 'Vadonut',
 image: '/assets/images/vadonut.png',
 category: 'appetizer',
 featured: false,
 label: 'New',
 price: '1.99',
 description: 'A quintessential ConFusion experience, is it a vada or is it a donut?',
 comments: [
 {
 rating: 5,
 comment: 'Imagine all the eatables, living in conFusion!',
 author: 'John Lemon',
 date: '2012-10-16T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Sends anyone to heaven, I wish I could get my mother-in-law to eat it!',
 author: 'Paul McVites',
 date: '2014-09-05T17:57:28.556094Z'
 },
 {
 rating: 3,
 comment: 'Eat it, just eat it!',
 author: 'Michael Jaikishan',
 date: '2015-02-13T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Ultimate, Reaching for the stars!',
 author: 'Ringo Starry',
 date: '2013-12-02T17:57:28.556094Z'
 },
 {
 rating: 2,
 comment: 'It\'s your birthday, we\'re gonna party!',
 author: '25 Cent',
 date: '2011-12-02T17:57:28.556094Z'
 }
 ]
 },
 {
 id: '3',
 name: 'ElaiCheese Cake',
 image: '/assets/images/elaicheesecake.png',
 category: 'dessert',
 featured: false,
 label: '',
 price: '2.99',
 description: 'A delectable, semi-sweet New York Style Cheese Cake, with Graham cracker crust and spiced with Indian cardamoms',
 comments: [
 {
 rating: 5,
 comment: 'Imagine all the eatables, living in conFusion!',
 author: 'John Lemon',
 date: '2012-10-16T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Sends anyone to heaven, I wish I could get my mother-in-law to eat it!',
 author: 'Paul McVites',
 date: '2014-09-05T17:57:28.556094Z'
 },
 {
 rating: 3,
 comment: 'Eat it, just eat it!',
 author: 'Michael Jaikishan',
 date: '2015-02-13T17:57:28.556094Z'
 },
 {
 rating: 4,
 comment: 'Ultimate, Reaching for the stars!',
 author: 'Ringo Starry',
 date: '2013-12-02T17:57:28.556094Z'
 },
 {
 rating: 2,
 comment: 'It\'s your birthday, we\'re gonna party!',
 author: '25 Cent',
 date: '2011-12-02T17:57:28.556094Z'
 }
 ]
 }
];

```

###### Updating the Menu Component 
-   Open menu.component.ts file and update its content, first by deleting the dishes constant and then make the following changes:

```js
import { Component, OnInit } from '@angular/core';
import { Dish } from '../shared/dish';
import { DISHES } from '../shared/dishes';
  
. . .
  
export class MenuComponent implements OnInit {
  
 dishes: Dish[] = DISHES;
  
 selectedDish: Dish;
. . .
  
 onSelect(dish: Dish) {
 this.selectedDish = dish;
 }
  
}
```

-   Then update the menu.component.html file as follows:

```html
. . .
  
 <mat-grid-tile *ngFor="let dish of dishes" (click) = "onSelect(dish)">
 . . .
 <app-dishdetail [dish] = "selectedDish"></app-dishdetail>
. . .
```

###### Updating Dish Detail Component 
-   Open dishdetail.component.ts and update its contents as follows:

```js
import { Component, OnInit, Input } from '@angular/core';
import { Dish } from '../shared/dish';
  
. . .
  
export class DishdetailComponent implements OnInit {
  
 @Input()  //<--- this is a decorator
 dish: Dish;
  
. . .
```

-   Save the changes and do a Git commit with the message "Data Binding".



#### Angular Service Basics 
##### Objectives and Outcomes 
In this lesson you will learn about the basics of Angular services and how they interact with Angular components. You will also learn the basics of Model-View-Controller (MVC) and Model-View-ViewModel (MVVM) software engineering paradigms. You will also be introduced to the basics of Dependency Injection (DI). At the end of this course you will be able to:

-   Add an Angular service and inject into a module and make use of it in the components.
    
-   Understand the basics of MVC and MVVM, and DI.


##### Generating a service 
use command: `ng generate service <service name>`

##### Dependency Injection
Dependency injection is a Software design pattern that implements inversion of control for resolving dependencies: 
- Dependency: an object that can be used (a service)
- Injection: Passing of a dependency to a dependent object so that it can use it. The client does not need to build the object 

Three ways for a component to get hold of its dependencies: 
- Create dependency using new operator
- Look up dependency using a global variable 
- Have dependency passed to where it is needed 

The third option is the most flexible 
- Hard coding of dependency avoided 
- testing becomes feasible 

Dependency injection involves four roles: 
- The service 
- The client
- The interfaces
- The injector 
##### Service Example
###### Objectives and Outcomes 
In this exercise you will create a new Angular service and inject it into your application. You will then make use of the service in the components. At the end of this exercise you will be able to:

-   Implement a service and inject into your application
    
-   Make use of the service in a component


###### Adding a Service 
-   Create a folder named _services_ in the _src/__app_ folder.
    
-   To add a service to your application using Angular CLI, type the following at the prompt:

`ng generate service services/dish`

-   This will create two new files in the services folder named dish.service.ts and dish.service.spec.ts.
    
-   Open dish.service.ts and update its contents as shown below:

```js
. . .
  
import { Dish } from '../shared/dish';
import { DISHES } from '../shared/dishes';
  
. . .
  
 getDishes(): Dish[] {
 return DISHES;
 }
. . .
```

-   Then add the service to the app.module.ts file as follows:

```js
. . .
  
import { DishService } from './services/dish.service';
  
@NgModule({
. . .
  
 providers: [DishService],
  
. . .
```


###### Using the Service 
-   Now update menu.component.ts file to make use of the service as follows:

```js
. . .
  
import { DishService } from '../services/dish.service';
  
. . .
  
export class MenuComponent implements OnInit {
  
 dishes: Dish[];
  
 selectedDish: Dish;
  
 constructor(private dishService: DishService) { }
 ngOnInit() {
 this.dishes = this.dishService.getDishes();
 }
  
. . .
  
}
```

-   Check that your application is still working correctly in the browser. Do a Git commit with the message "Basic Service".

### Week 3
#### Angular Forms, Angular and Reactive JavaScript
In this module we study Angular support for forms and form validation. Both template-driven forms and reactive forms will be introduced. You will also learn about Promises. Then you will learn briefly about reactive programming, RxJs and its use in Angular.
#### Learning Objectives 
-   Create template-driven forms and reactive forms in an Angular application
-   Demonstrate an understanding of reactive programming
-   Use RxJS to support reactive programming in Angular applications
-   Demonstrate the use of observables and reactive approaches in Angular applications
#### Angular Template-driven Forms
In this lesson you will learn about Angular template-driven forms. You will construct template-driven forms and learn about form validation. At the end of this lesson you will be able to:

-   Construct an Angular template-driven form and use it within your Angular application to enable user input
    
-   Validate the information entered into the form fields using the form validation support provided in Angular
##### Exercise: Dialogs
- find a way to overlay content on top of the webpage 

###### Objectives and Outcomes 
In this exercise you will learn to use the Angular material dialog component to show a dialog view in the Angular application. At the end of this exercise you will be able to:

-   Add a dialog view using the Angular Material dialog component to your application


###### Triggering the Dialog View
-   Add a link to the toolbar in the header component, which when clicked will open a Login form in a dialog view:

```html
<span class="flex-spacer"></span>
<a mat-button (click)="openLoginForm()"><span class="fa fa-sign-in fa-lg"></span> Login</a>

```


###### Adding a Dialog Component
-   Next create an Angular component named LoginComponent to your Angular application:

```bash
ng g component login
```

-   To make this component into a Dialog component, open login.component.ts and import MatDialog and MatDialogRef as follows:

```ts
import {MatDialog, MatDialogRef} from '@angular/material';

```

-   Then update the template file login.component.html as follows:

```html
<mat-toolbar color="primary">

 Login

 <span class="flex-spacer"></span>

 <button mat-button mat-dialog-close>&times;</button>

</mat-toolbar>
```

-   To make this component be opened from another component, you need to declare this as an EntryComponent in the AppModule, by adding the following to the NgModule decorator. In addition you need to import the MatDialogModule;

```ts
. . .
  
import { MatDialogModule } from '@angular/material/dialog';
  
. . .
  
@NgModule({
. . .
  
 imports: [
 . . .,
 MatDialogModule,
 . . .
 ],
 . . .
 entryComponents: [
 LoginComponent
 ],
. . .
})
```

-   Now, to trigger the Dialog view of the Login component, open header.component.ts and update it as follows:

```ts
. . .
  
import { MatDialog, MatDialogRef } from '@angular/material';
import { LoginComponent } from '../login/login.component';
  
. . .
  
export class HeaderComponent implements OnInit {
  
 constructor(public dialog: MatDialog ) { }
  
 ngOnInit() {
 }
  
 openLoginForm() {
 this.dialog.open(LoginComponent, {width: '500px', height: '450px'});
 }
  
}
```


##### Exercise: Angular Template-driven Forms
###### Objectives and Outcomes 
In this exercise you will learn about using Angular template-driven forms in your Angular application. At the end of this exercise you will be able to:

-   Design a template-driven form in your Angular application.


###### Add in the Login Template-driven Form
-   To use the Template-driven forms, import the Angular Forms module into app.module.ts by updating it as follows:

```ts
. . .
  
import { MatFormFieldModule } from '@angular/material/form-field';
import { MatInputModule } from '@angular/material/input';
import { MatCheckboxModule } from '@angular/material/checkbox';
import { FormsModule } from '@angular/forms'; 
  
. . . 
  
@NgModule({ 
. . . 
  
 imports: [ 
 . . .
 MatFormFieldModule, 
 MatInputModule,
 MatCheckboxModule,
 . . .
 FormsModule 
 ],
. . .
```

- open your previously created dialog component html file and add in the form as follows: 


###### Objectives and Outcomes - Validation
In this exercise you will learn about adding form validation to your template-driven forms in Angular. You will show validation error messages to the users within the form. At the end of this exercise you will be able to:

-   Add in form validation support to your template-driven forms
    
-   Show validation error messages to the users


###### Adding Template Reference Variables 
-   Open login.component.html file and add in the template reference variables to the two `<input>` elements and the `<form>` element as follows:
```html
. . .
<form novalidate #loginForm="ngForm" (ngSubmit)="onSubmit()">
  
. . .
  
 <input matInput placeholder="Username" type="text"[(ngModel)]="user.username" name="username" #username="ngModel" required>
. . .
  
 <input matInput placeholder="Password" type="password" [(ngModel)]="user.password" name="password" #password="ngModel" required>
. . .
```
	


###### Doing Form Validation
-   You can now disable the submit button if the form is invalid as follows:

```html
. . .
 <button type="submit" mat-button class="background-primary text-floral-white" [disabled]="loginForm.form.invalid" >Login</button>
. . .
```






#### Angular Reactive forms 
##### Objectives and Outcomes 
In this lesson you will learn to create reactive forms in your Angular application. You will also be able to perform form validation using the validation support for reactive forms. At the end of this lesson you will be able to:

-   Add a form to your Angular application using reactive forms.
    
-   Add form validation to your reactive Angular forms


##### Angular Reactive Forms Part 1
###### Objectives and Outcomes 
In this exercise you will learn about using Angular reactive forms in your Angular application. At the end of this exercise you will be able to:

-   Design a reactive form in your Angular application.


###### Importing the Reactive Forms Module 
-   You will start out by importing the ReactiveFormsModule from @angular/forms into your AppModule as follows:

```ts
. . .
import { MatSelectModule } from '@angular/material/select';
import { MatSlideToggleModule } from '@angular/material/slide-toggle';
import { ReactiveFormsModule } from '@angular/forms';
  
. . .
  
@NgModule({
. . .
  
 imports: [
 . . .
 MatSelectModule,
 MatSlideToggleModule,
 . . .,
 ReactiveFormsModule
 ],
 . . .
```

-   You will then create a new file named feedback.ts in the shared folder and update its contents as follows:

```ts
export class Feedback {
 firstname: string;
 lastname: string;
 telnum: number;
 email: string;
 agree: boolean;
 contacttype: string;
 message: string;
};
  
export const ContactType = ['None', 'Tel', 'Email'];
```


###### Creating the Reactive Form 
-   Open the contact.component.ts file and update it as follows to create the reactive form in the code:

```ts
. . .
import { FormBuilder, FormGroup, Validators } from '@angular/forms';
import { Feedback, ContactType } from '../shared/feedback';
  
. . .
  
export class ContactComponent implements OnInit {
  
 feedbackForm: FormGroup;
 feedback: Feedback;
 contactType = ContactType;
  
 constructor(private fb: FormBuilder) {
 this.createForm();
 }
  
 ngOnInit() {
 }
  
 createForm() {
 this.feedbackForm = this.fb.group({
 firstname: '',
 lastname: '',
 telnum: 0,
 email: '',
 agree: false,
 contacttype: 'None',
 message: ''
 });
 }
  
 onSubmit() {
 this.feedback = this.feedbackForm.value;
 console.log(this.feedback);
 this.feedbackForm.reset();
 }
  
}
```

-   Then open contact.component.html and add the reactive form to it as follows:

```html
 <div fxFlex fxFlexOffset="20px" class="form-size">
 <h3>Send us your Feedback</h3>
 <p>{{ feedbackForm.value | json }} {{ feedbackForm.status | json }}</p>
  
 <form novalidate [formGroup]="feedbackForm" (ngSubmit)="onSubmit()">
 <p>
 <mat-form-field class="half-width">
 <input matInput formControlName="firstname" placeholder="First Name" type="text">
 </mat-form-field>
 <mat-form-field class="half-width">
 <input matInput formControlName="lastname" placeholder="Last Name" type="text">
 </mat-form-field>
 </p>
 <p>
 <mat-form-field class="half-width">
 <input matInput formControlName="telnum" placeholder="Tel. Number" type="tel">
 </mat-form-field>
 <mat-form-field class="half-width">
 <input matInput formControlName="email" placeholder="Email" type="email">
 </mat-form-field>
 </p>
 <table class="form-size">
 <td>
 <mat-slide-toggle formControlName="agree">May we contact you?</mat-slide-toggle>
 </td>
 <td>
 <mat-select placeholder="How?" formControlName="contacttype">
 <mat-option *ngFor="let ctype of contactType" [value]="ctype">
 {{ ctype }}
 </mat-option>
 </mat-select>
 </td>
 </table>
 <p>
 <mat-form-field class="full-width">
 <textarea matInput formControlName="message" placeholder="Your Feedback" rows=12></textarea>
 </mat-form-field>
 </p>
 <button type="submit" mat-button class="background-primary text-floral-white">Submit</button>
 </form>
 </div>
```

-   Add the following CSS classes to contact.component.scss file:

```css
.full-width {
 width: 95%
}
  
.half-width {
 width: 45%
}
  
.form-size {
 width: 75%
}
```


##### Angular Reactive Forms Part 2
###### Objectives and Outcomes 
In this exercise you will learn about adding form validation to your reactive forms in Angular. You will show validation error messages to the users within the form. At the end of this exercise you will be able to:

-   Add in form validation support to your reactive forms
    
-   Show validation error messages to the users


###### Add Form Validation
-   Open contact.component.ts and update the Form Model as shown below:

```ts
import { Component, OnInit, ViewChild } from '@angular/core';
  
. . .
  
export class ContactComponent implements OnInit {
  
 @ViewChild('fform') feedbackFormDirective;
  
. . .
 
  
 createForm() {
 this.feedbackForm = this.fb.group({
 firstname: ['', Validators.required ],
 lastname: ['', Validators.required ],
 telnum: ['', Validators.required ],
 email: ['', Validators.required ],
 agree: false,
 contacttype: 'None',
 message: ''
 });
 }
  
 onSubmit() {
 this.feedback = this.feedbackForm.value;
 console.log(this.feedback);
 this.feedbackForm.reset({
 firstname: '',
 lastname: '',
 telnum: '',
 email: '',
 agree: false,
 contacttype: 'None',
 message: ''
 });
 this.feedbackFormDirective.resetForm();
 }
. . .
```


-   Update the form in the contact.component.html file as follows:

```html
. . .
  
 <form novalidate [formGroup]="feedbackForm" #fform="ngForm" (ngSubmit)="onSubmit()">
 <p>
 <mat-form-field class="half-width">
 <input matInput formControlName="firstname" placeholder="First Name" type="text" required>
 <mat-error *ngIf="feedbackForm.get('firstname').hasError('required') && feedbackForm.get('firstname').touched">First name is required</mat-error>
 </mat-form-field>
 <mat-form-field class="half-width">
 <input matInput formControlName="lastname" placeholder="Last Name" type="text" required>
 <mat-error *ngIf="feedbackForm.get('lastname').hasError('required') && feedbackForm.get('lastname').touched">Last name is required</mat-error>
 </mat-form-field>
 </p>
 <p>
 <mat-form-field class="half-width">
 <input matInput formControlName="telnum" placeholder="Tel. Number" type="tel" required>
 <mat-error *ngIf="feedbackForm.get('telnum').hasError('required') && feedbackForm.get('telnum').touched">Tel. number is required</mat-error>
 </mat-form-field>
 <mat-form-field class="half-width">
 <input matInput formControlName="email" placeholder="Email" type="email" required>
 <mat-error *ngIf="feedbackForm.get('email').hasError('required') && feedbackForm.get('email').touched">Email ID is required</mat-error>
 </mat-form-field>
 </p>
. . .
```


#### Angular and Promise 
##### Angular and Promise: Objectives and Outcomes
In this lesson we briefly review JavaScript promises and then see how we can redesign the services to return promises instead of returning the values immediately. At the end of this lesson you will be able to:

-   Get a basic understanding of JavaScript promises
    
-   Use promises to enable the services to function asynchronously and return results when available
##### What are promises?
They try to make asynchronous computation easier to accomplish or understand as someone who is used to synchronus computing 

You should be able to proceed forward without waiting for a result, for example, you call a service and don't get the data for a few ms. 

Promises provide us with a way of dealing with this. 

Promises are a proxy for a value not necessarily known when the promise is created: 
- it represents a value that may be available now, or in the future, or never


Look into Promises more when you need them

#### Angular and [[RxJS]]
##### Objectives and Outcomes
In this lesson we will examine the combination of Angular and RxJS, the reactive JavaScript frameworks. We will also examine some observables that are already built into the Angular framework and how we can leverage them to do reactive programming within Angular. At the end of this lesson you will be able to:

-   Get a working overview of reactive programming, the observer pattern and the use of observables in Angular
    
-   Make use of the Angular support for observables to do reactive Angular applications


