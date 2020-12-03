# `<Login />` and `<Auth />`

1. **Why is the Context API useful?**

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

2. **Can a component outside of a provider get its context?**

No, every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.

3. **What are some common use cases for using the Context API?**

Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

4. **Describe “Context Hell”**

there are two popular types of sharing logic in components which are Higher-Order Components and Rendering Props. When your applications have a massive quantity of nested Components, they will cause a “Wrapper Hell.”

React Hooks vs. Wrapper Hell
Term

## Vocabulary Terms

### global state
keeping a state at the top level and provide access methods to all child levels without the need to pass props.
### global context
React's context allows you to share information to any component, by storing it in a central place and allowing access to any component that requests it (usually you are only able to pass data from parent to child via props).
### provider
The provider acts as a delivery service. When a consumer asks for something, it finds it in the context and delivers it to where it's needed.
### consumer
A consumer is where the stored information ends up. It can request data via the provider and manipulate the central store if the provider allows it.

----

* [What is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)
* [React-cookies component](https://www.npmjs.com/package/react-cookies)
* [React-cookie library](https://www.npmjs.com/package/react-cookie)
* [Provider Pattern with react context API](https://blog.flexiple.com/provider-pattern-with-react-context-api/)
* [Working with react context API](https://www.toptal.com/react/react-context-api)
