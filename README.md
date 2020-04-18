# angular-workshop-team5
## Introduction
Angular is an app-design framework and development platform for creating efficient and sophisticated single-page apps. Angular is a complete rewrite from the same team that built AngularJS.The architecture of an Angular application relies on certain fundamental concepts. The basic building blocks are NgModules, which provide a compilation context for components. NgModules collect related code into functional sets; an Angular app is defined by a set of NgModules. An app always has at least a root module that enables bootstrapping, and typically has many more feature modules.

Components define views, which are sets of screen elements that Angular can choose among and modify according to your program logic and data.

Components use services, which provide specific functionality not directly related to views. Service providers can be injected into components as dependencies, making your code modular, reusable, and efficient.

## Folder Structure
[Angular folder structure](https://www.youtube.com/watch?v=_TLhUCjY9iA&feature=youtu.be)

    > e2e

    > node_modules

    > src

        > app

        > assets

        > environments

        ..index.html
  
        ..styles.scss

1. The e2e folder is for end to end testing. We won't be covering testing in this course, but I will do a separate tutorial on that.
1. node_modules is a folder you will never watch to touch, as it contains the project's dependencies.
1. src contains much of your code.
1. app is where you will spend the most of your time writing your Angular 8 code. It includes the routing, components, and more.
1. index.html is the entry point to the app, and you generally don't touch this file.
1. styles.scss is where your global CSS rulesets will reside.





## Components and Two-way Binding
[Components](https://www.youtube.com/watch?v=23o0evRtrFI)

The fundamental building blocks of your Angular app are the components. Components consist of 3 elements:

- The imports
- The component decorator, which are various properties for your component. The component decorator includes locations to your component's template and CSS location.
- The component logic, where your code resides.


 import { Component } from '@angular/core';

 @Component
 
 ({

    selector: 'app-root',

    templateUrl: './app.component.html',

    styleUrls: ['./app.component.scss']

 })

 export class AppComponent 

{

  title = 'myapp';

}


[Two-way Binding](https://www.youtube.com/watch?v=DOWwWsbG1Sw)

Every Angular application has at least one component, the root component that connects a component hierarchy with the page document object model (DOM). Each component defines a class that contains application data and logic, and is associated with an HTML template that defines a view to be displayed in a target environment.

The @Component() decorator identifies the class immediately below it as a component, and provides the template and related component-specific metadata.A template combines HTML with Angular markup that can modify HTML elements before they are displayed. Template directives provide program logic, and binding markup connects your application data and the DOM. 

There are two types of data binding:

Event binding lets your app respond to user input in the target environment by updating your application data.
Property binding lets you interpolate values that are computed from your application data into the HTML.
Before a view is displayed, Angular evaluates the directives and resolves the binding syntax in the template to modify the HTML elements and the DOM, according to your program data and logic. Angular supports two-way data binding, meaning that changes in the DOM, such as user choices, are also reflected in your program data.

 Templates can use pipes to improve the user experience by transforming values for display. For example, use pipes to display dates and currency values that are appropriate for a user's locale. Angular provides predefined pipes for common transformations, and you can also define your own pipes.

## Angular App Fetch Calls
 

