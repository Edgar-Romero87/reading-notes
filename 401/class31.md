# Hooks API

1. Why do we not need more .html pages in a multi-page React app?

In Multi-page apps, we get back multiple HTML pages, where each page has content for given Router.

2. If we wanted a component to show up on every page, where would we put it and why?

- Inside the `<BrowserRouter />`, outside a `<Route />`

3. What does props.children contain?

Used to display whatever you include between the opening and closing tags when invoking a component.

## Vocabulary Terms
### Composition
Composition is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components.
### Children / Child Components
A child component is a more specific part inside a parent component. Example would be a parent component being a PERSON. ARMS and LEGS are child components of it.
### Hash Routing
It uses URL hash, it puts no limitations on supported browsers or web server. Server-side routing is independent from client-side routing.
### Link Routing
- Provides declarative, accessible navigation around your application.
- The primary way to allow users to navigate around your application. will render a fully accessible anchor tag with the proper href.
- A can know when the route it links to is active and automatically apply an activeClassName and/or activeStyle when given either prop. The will be active if the current route is either the linked route or any descendant of the linked route. To have the link be active only on the exact linked route, use instead or set the onlyActiveOnIndex prop.

----
- [Making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)
- [The state hook](https://reactjs.org/docs/hooks-state.html)
- [Hooks API](https://reactjs.org/docs/hooks-overview.html)
- [Hooks API reference](https://reactjs.org/docs/hooks-reference.html)
- [Effects hook](https://reactjs.org/docs/hooks-effect.html)
