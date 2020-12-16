# Redux - Asynchronous Actions

1. **How granular should your reducers be?**

Reducers should be granular to avoid repeating yourself on simple actions and write dry code.

2. **Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched**

- many reducers can react to a single actions, a single reducer can react to multiple actions
- Pro for small apps: helps keep our code organized and our state separated by concern, it also gives us the ability to have multiple reducers have the same action. Source: [Share actions across multiple reducers in Redux](https://medium.com/@thomasmarren/share-actions-across-multiple-reducers-in-redux-e359a75f2242)

3. **Name a strategy for preventing the above**

Many reducers may handle one action. One reducer may handle many actions. Putting them together negates many benefits of how Flux and Redux application scale. This leads to code bloat and unnecessary coupling. You lose the flexibility of reacting to the same action from different places, and your action creators start to act like “setters”, coupled to a specific state shape, thus coupling the components to it as well. Soruce: [Reducers and action creators aren't a one-to-one mapping ](https://github.com/pitzcarraldo/reduxible/issues/8) 

## Vocabulary Terms

### Store
A store holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it. A store is not a class. It's just an object with a few methods on it. To create it, pass your root reducing function to createStore.
### Combined reducers
The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

----

## Preparation Materials

* [Async Actions](https://redux.js.org/advanced/async-actions)

* [Thunk Middleware](https://github.com/reduxjs/redux-thunk)

* [Redux Thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)