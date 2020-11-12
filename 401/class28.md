# Component Composition

1. **Can a parent component access the state of a child component?**

Yes, a parent can access the state of a child through a callback function like onClick, onChange, or React componentDidUpdate. Source: [Linguinecode](https://linguinecode.com/post/get-child-component-state-from-parent-component)

2. **What can be passed along in a prop variable?**

Data(objects with key value pairs)

3. **How can a child component “know” the state of another component?**

Props are data that are passed from a parent to its children and are made available through this.props on the child component.
## Vocabulary Terms

### Component props
When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object “props”.
### Component state
The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.
### Application state
This is the state of an application as a whole. Unlike component state which is specific to that component, application state is global and can be accessed by any component within the application.

----
[React Basics Recap](https://www.freecodecamp.org/news/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030/)

[props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

[Composition vs Inheritance](https://canvas.instructure.com/courses/2168372/discussion_topics/9374383)

[React testing library api example](https://testing-library.com/docs/react-testing-library/example-intro/)

## Bookmark
[React-if component](https://www.npmjs.com/package/react-if)

[React-testing-library-async](https://testing-library.com/docs/dom-testing-library/api-async/)
