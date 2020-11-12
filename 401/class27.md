# Props and State

1. **Does a deployed React application require a server?**

React. js does not use a webserver to create virtual DOMs. It builds the virtual DOM and does its diff operations on the client's browser.

2. **Why do we prefer to test a React application at the behavior rather than the unit level?**

Because then we can test the actual interaction the user is having with the React components rather than testing what is "under the hood".

3. **What does `npm run build` do?**

`npm run build` does nothing unless you specify what "build" does in your package.json file. It lets you perform any necessary building/prep tasks for your project, prior to it being used in another project. `npm run build`: runs the build field from the `package.json` `scripts` field

4. **Describe the actual composition/architecture of a React application**

React - a popular front-end technology like AngularJS - is a Javascript framework, but it only works with the View layer, which means you have only the **V** in the **MVC - Model-View-Controller - architecture**. React gives you the template language and a few function hooks to render HTML.

## Vocabulary Terms
### BDD
Behavior Driven Development (BDD) is a branch of Test Driven Development (TDD). BDD uses human-readable descriptions of software user requirements as the basis for software tests. ... Each test is based on a user story written in the formally specified ubiquitous language based on English.
### Acceptance Tests
An acceptance test is a formal description of the behavior of a software product, generally expressed as an example or a usage scenario.
### mounting
"Mounting" is when React "renders" the component for the first time and actually builds the initial DOM from those instructions.
### build
In software development, a build is the process of converting source code files into standalone software artifact that can be run on a computer, or the result of doing so.

----

[setState Explained](https://css-tricks.com/understanding-react-setstate/).

[Handling Events](https://reactjs.org/docs/handling-events.html).

[Forms](https://reactjs.org/docs/forms.html).

[State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html).

[Components and Props](https://reactjs.org/docs/components-and-props.html).

[RTL Testing Example](https://thomlom.dev/beginner-guide-testing-react-apps/).

[Roles Reference](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques#Roles).