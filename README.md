# Section 1: Getting Started

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.1.5.

## Project Setup and First app

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

![angular-first-1](images/angular-first-1.png)
![angular-first-2](images/angular-first-2.png)
![angular-first-3](images/angular-first-3.png)
![angular-first-4](images/angular-first-4.png)
![angular-first-5](images/angular-first-5.png)
![angular-first-6](images/angular-first-6.png)
![angular-first-7](images/angular-first-7.png)
![angular-first-8](images/angular-first-8.png)

## A basic project setup using Bootstrap for styling

```shell
npm install --save bootstrap@3
```

![angular-first-9](images/angular-first-9.png)
![angular-first-10](images/angular-first-10.png)

## How an Angular App gets loaded and started

![basic-1](images/basic-1.png)
![basic-2](images/basic-2.png)
![basic-3](images/basic-3.png)

## Components are important
Components are the main building block for Angular applications. Each component consists of:

- An HTML template that declares what renders on the page
- A TypeScript class that defines behavior
- A CSS selector that defines how the component is used in a template
- Optionally, CSS styles applied to the template

![basic-4](images/basic-4.png)

## Creating a New Component
- Create the new folder (app/server)
- Create the file (server.component.ts)

![basic-5](images/basic-5.png)

## Understanding the role of AppModule and Component
![basic-6](images/basic-6.png)

## Using Custom Components
![basic-7](images/basic-7.png)

## Creating components with the CLI & Nesting Components
```shell
ng generate component servers
ng g c servers
```
![create-component-cli-1](images/create-component-cli-1.png)
![create-component-cli-2](images/create-component-cli-2.png)
![create-component-cli-3](images/create-component-cli-3.png)
![create-component-cli-4](images/create-component-cli-4.png)
![create-component-cli-5](images/create-component-cli-5.png)
![create-component-cli-6](images/create-component-cli-6.png)

## Working with component templates
![component-style-1](images/component-style-1.png)

## Working with Component styles
![component-styles-1](images/component-styles-1.png)

## Fully understanding the Component Selector
![component-selector-1](images/component-selector-1.png)

## What is Databinding?
![data-binding-1](images/data-binding-1.png)

## String Interpolation
![string-interpolation-1](images/string-interpolation-1.png)

## Property Binding
Property binding is a one-way mechanism that lets you set the property of a view element. It involves updating the value of a property in the component and binding it to an element in the view template.
![property-binding-1](images/property-binding-1.png)

## Property Binding vs String Interpolation
![pb-si-1](images/pb-si-1.png)
![pb-si-2](images/pb-si-2.png)

## Event Binding
![event-binding-1](images/event-binding-1.gif)

## Bindable Properties and Events
How do you know to which Properties or Events of HTML Elements you may bind? You can basically bind to all Properties and Events - a good idea is to console.log()  the element you're interested in to see which properties and events it offers.

Important: For events, you don't bind to onclick but only to click (=> (click)).

The MDN (Mozilla Developer Network) offers nice lists of all properties and events of the element you're interested in. Googling for YOUR_ELEMENT properties  or YOUR_ELEMENT events  should yield nice results.

## Passing and Using Data with Event Binding
![passing-using-1](images/passing-using-1.png)
![passing-using-2](images/passing-using-2.png)
![passing-using-3](images/passing-using-3.png)
![passing-using-4](images/passing-using-4.gif)

## Important: FormsModule is required for Two-Way-Binding
Important: For Two-Way-Binding (covered in the next lecture) to work, you need to enable the ngModel  directive. This is done by adding the FormsModule  to the imports[]  array in the AppModule.

You then also need to add the import from @angular/forms  in the app.module.ts file:

import { FormsModule } from '@angular/forms'; 

## Two-Way-Databinding
![two-way-1](images/two-way-1.png)
![two-way-2](images/two-way-2.png)

## Combining all Forms of Databinding
![combining-databinding-1](images/combining-databinding-1.png)
![combining-databinding-2](images/combining-databinding-2.png)

## What are Directives?

Directives are Instructions in the DOM!

Directives are classes that add new behavior or modify the existing behavior to the elements in the template.

Basically directives are used to manipulate the DOM, for example adding/removing the element from DOM or changing the appearance of the DOM elements.

- Types of directives

1. Component directive
Components are special directives in Angular. They are the directive with a template

It might confuse you a bit, but if you see the definition of the directive, it says directives are used to manipulate the DOM, so now if you think what component is doing, it is actually showing something in DOM, hence we can say component is also a directive with a template (template or templateUrls).

2. Structural directive
Structural directives are used to change the DOM layout by adding and removing DOM elements. It basically changes the structure of the DOM
Examples of structural directives are ngIf, ngFor, ngSwitch.

*ngIf — adds or removes element from DOM.
*ngFor — renders list of elements on every iteration.

All structural Directives are preceded by Asterix (*)symbol.

3. Attribute directive
Attribute directives are used to change the appearance or behavior of an element.

Examples of attributes directives are ngStyle, ngClass, ngModel

ngStyle — used to apply styles that will change the appearance.
ngClass — used to apply CSS classes to change the appearance.

## Using nglf to Output Data Conditionally
![ngif-1](images/ngif-1.png)
![ngif-2](images/ngif-2.png)
![ngif-3](images/ngif-3.gif)
![ngif-4](images/ngif-4.png)

## Enhancing nglf with an Else Condition
![ng-if-else-1](images/ng-if-else-1.png)

## Styling Elements Dynamically with ngStyle
Unlike structural directives, attribute directives don't add or remove elements. They only change the element they were placed on.

![ng-style-1](images/ng-style-1.png)
![ng-style-2](images/ng-style-2.png)
![ng-style-3](images/ng-style-3.png)
![ng-style-4](images/ng-style-4.png)

## Applying CSS Classes Dynamically with ngClass
![ng-class-1](images/ng-class-1.png)
![ng-class-2](images/ng-class-2.png)
![ng-class-3](images/ng-class-3.png)

## Outputting Lists with ngFor
![ngfor-1](images/ngfor-1.png)
![ngfor-2](images/ngfor-2.png)
![ngfor-3](images/ngfor-3.gif)
