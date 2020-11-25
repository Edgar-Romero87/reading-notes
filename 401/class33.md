# Context API

1. **Describe use cases for `useMemo()` and `useReducer()`**
- Returns a `memoized` value.
Pass a “create” function and an array of dependencies. `useMemo` will only recompute the memoized value when one of the dependencies has changed. This optimization helps to avoid expensive calculations on every render.
Remember that the function passed to `useMemo` runs during rendering. Don’t do anything there that you wouldn’t normally do while rendering.
- `useReducer` is usually preferable to `useState` when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. `useReducer` also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.
Source: [Reactjs](https://reactjs.org/docs/hooks-reference.html#usememo)

2. **Why do custom hooks need the use prefix?**

Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it. Source: [Reactjs](https://reactjs.org/docs/hooks-reference.html#usememo)

3. **What do custom hooks usually do?**

A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.

4. **Using any list of custom hooks, research and name one that you think will be useful in your applications**
The function passed to useEffect will run after the render is committed to the screen. Think of effects as an escape hatch from React’s purely functional world into the imperative world.

5. **Describe how a hook that fetches API data might work**

## Vocabulary Terms

### Reducer
A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently.

----

## Preparation Materials

- [Context API](https://reactjs.org/docs/context.html)
- [Hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
- [React context links](https://github.com/diegohaz/awesome-react-context)
