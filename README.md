# binding-syntax

In Angular, the term "binding syntax" refers to the way you can bind data from your component's code to your template, allowing you to dynamically update and display data in your application's user interface.

Angular provides several types of binding syntax, including:

## Interpolation ({{}}):
Interpolation allows you to insert the value of a component's property directly into the template. You can use double curly braces ({{}}) to surround the property you want to display. For example:

```typescript
<h1>{{ title }}</h1>
```

In this example, the value of the component's title property will be dynamically inserted into the h1 tag.

## Property binding ([property]):
Property binding allows you to set the value of an HTML element's property to the value of a component's property. To bind a property, you use square brackets ([property]) and assign the component's property to it. For example:

```typescript
<input [value]="name">
```
  
In this case, the value property of the <input> element is bound to the name property of the component. Any changes to the name property will automatically update the value of the input field.

## Event binding ((event)):
Event binding allows you to respond to user events, such as button clicks or input changes. You use parentheses to surround the event name and assign a method from the component to it. For example:

```typescript
<button (click)="onClick()">Click me</button>
```
  
In this example, the click event of the <button> element is bound to the onClick() method of the component. When the button is clicked, the onClick() method will be executed.

## Two-way binding ([(ngModel)]):
Two-way binding combines both property binding and event binding to create a two-way data flow between the component and the template. It allows you to update the component's property when the user interacts with the template and vice versa. To use two-way binding, you typically use the ngModel directive along with square brackets and parentheses. For example:

```typescript
<input [(ngModel)]="name">
```

In this case, the ngModel directive is used to bind the value of the <input> element to the name property of the component. Any changes to the input field will update the name property, and any changes to the name property will update the input field.

These are just some examples of the binding syntax in Angular. You can use these binding techniques to create dynamic and interactive applications by connecting your component's data to your template.
