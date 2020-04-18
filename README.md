# angular-workshop-team5
## Introduction
Angular is an app-design framework and development platform for creating efficient and sophisticated single-page apps. Angular is a complete rewrite from the same team that built AngularJS.The architecture of an Angular application relies on certain fundamental concepts. The basic building blocks are NgModules, which provide a compilation context for components. NgModules collect related code into functional sets; an Angular app is defined by a set of NgModules. An app always has at least a root module that enables bootstrapping, and typically has many more feature modules.

Components define views, which are sets of screen elements that Angular can choose among and modify according to your program logic and data.

Components use services, which provide specific functionality not directly related to views. Service providers can be injected into components as dependencies, making your code modular, reusable, and efficient.

## Folder Structure
[Angular folder structure](https://www.youtube.com/watch?v=_TLhUCjY9iA&feature=youtu.be)

## Components and Two-way Binding
[Components](https://www.youtube.com/watch?v=23o0evRtrFI)
[Two-way Binding](https://www.youtube.com/watch?v=DOWwWsbG1Sw)

Every Angular application has at least one component, the root component that connects a component hierarchy with the page document object model (DOM). Each component defines a class that contains application data and logic, and is associated with an HTML template that defines a view to be displayed in a target environment.

The @Component() decorator identifies the class immediately below it as a component, and provides the template and related component-specific metadata.A template combines HTML with Angular markup that can modify HTML elements before they are displayed. Template directives provide program logic, and binding markup connects your application data and the DOM. 

There are two types of data binding:

Event binding lets your app respond to user input in the target environment by updating your application data.
Property binding lets you interpolate values that are computed from your application data into the HTML.
Before a view is displayed, Angular evaluates the directives and resolves the binding syntax in the template to modify the HTML elements and the DOM, according to your program data and logic. Angular supports two-way data binding, meaning that changes in the DOM, such as user choices, are also reflected in your program data.

 Templates can use pipes to improve the user experience by transforming values for display. For example, use pipes to display dates and currency values that are appropriate for a user's locale. Angular provides predefined pipes for common transformations, and you can also define your own pipes.

## Angular App Fetch Calls
 

