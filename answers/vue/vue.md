# Vue Interview Answers

## What is VueJS?

VueJS is a client side JavaScript framework which allows developers to be more performant when developing web applications. In comparison with ReactJS VueJS has more structured arhictecture. In comparison with Angular VueJS is more flexible and leaves developers space for freedom.

## What is the difference between v-show and v-if directives?

`v-show` adds `display: none` CSS attribute to the element so that element disapears from web page but remains present in DOM. `v-if` completely removes element from DOM. `v-if` is more proper for situations when element does not switch very often. `v-show` otherwise is better in situations when element is toggled often because requires less perfomance for each toggling.

## Why do you need to use key attribute on for directive?

`key` attribute is used to uniquely indentify element in the list and to prevent unnecessary rebuilding. Usually it is better to use ID of the entity as a `key`.

## What are props?

Props are specific types of attributes which allows data to be passed down through the tree of components. Props are reactive meaning that changing the prop value will cause re-render of the component.

## How do you communicate from child to parent using events?

Events are another type of communication mechanism between components which allows data to be passed from child component to parent. Events are created by `emit` method which accepts event name and additional payload.

## How do you implement model on custom input components?

To implement two-way binding there must be a prop and event in the component. In component declaration special `model` object allows configuring the value and prop which will be used by `v-model` directive.

## What are slots?

Slots is a mechanism which allows child component manipulate data passed by parent component inside tags. By using slots child component can decide where to place (or not to place) data/markup provided by parent.

## What are mixins?

Mixin is a part of component logic placed outside. Mixin can extend component's configuration and allows to prevent code duplication by placing repetitive parts outside and reusing them. Mixins are considered as anti-patterns because they make the origins of some component's logic unclear.

## What is scoped CSS?

Scopes CSS is a special type of CSS code which applies only to current component and its children. Scoped CSS has no effect on parent and sibling elements.

## Why the component data must be a function?

While reading VueJS documentation you could notice that the example of simple app with single instance of application uses object as a data. In contrast, SFC (single file components) use function instead of object for data declaration. Usage of functions prevents sharing the same state between different instances of the same component. When having no components it is possible to use object because there are no other instances of component which can depend on this state.

## What are the lifecycle methods of VueJS?

`beforeCreate`, `created`, `beforeMount`, `mounted`, `beforeUpdate`, `updated`, `beforeUnmount` and `unmounted`.

## What is vue instance?

Is an instance of Vue application with scoped global context, components, store and so on.

## What are the conditional directives?

Conditional directives are directives which accepts boolean as a value to decide whether to render the element or not.

## Why should not use if and for directives together on the same element?

`v-if` has higher priority then `v-for` so usage of both directives together will causes error when data from `v-for` is used in `v-if`.

## What are the array detection mutation methods?

Usually modification of complex data types does not trigger re-render of the view so it is recommended to reassign value to manually notify about data change. In contrast, array detection mutation methods change initial array but allows reactive UI to be notified about changes.

## What is the purpose of v-for directive?

`v-for` directive is used to go through iterable instance and render piece of markup on each interation. For instance, `v-for` is needed when rendering a list of posts going through array of posts.

## What is vuex?

Vuex is one of two (the second is Pinia) primary global stores of VueJS ecosystem. It is used to make reactive data be directly accessible from everywhere in components tree. This mechanism eliminates the need to pass data and events through several components till reaching the target component.

## What are vuex getters?

There are two ways to retrieve data from Vuex global store. First using the direct access to state and the second is through getters. Getters are functions which ideally return and modify state into more comfortable for format for consumption.

## What are vuex mutations?

Mutations are SYNCHRONOUS functions which accept state and optionally additional payload and modifies state. The main reason of creation mutations was to make predictable and observable mechanism of state changing.

## How do you perform mutations in components?

Mutations can be executed in two ways. First, by calling `.commit` method of store object and passing mutation name as string. Second, by using `.mapMutatations` method from `vuex` package which add mutation method directly into scope of the component.

## What are vuex actions?

Because mutations are not allowed to be asynchronous there is another type of store functions which can perform asynchronous tasks. Actions have access to context and can be asynchronous. Usually after making asynchronous task actions call mutations through the context object.

## Give an example usage of actions?

In blog application actions can be used to perform asynchronous request to external API and then call mutation to set retrieved posts into state (from where posts will be accessible by UI).

## What are modules in vuex?

Modules are grouped set of actions, mutations, state and getters with specific namespace. Modules are used to decompose domains into separate similar parts.

## How do you represent one way data flow in vuex?

Actions are called from components. Actions always call mutations. Mutations change state. State is retrieved through getters by components.

## How do you display store state in vue components?

We can access state through `mapState` or `this.store.state`. Also, state data can be retrieved through getters rather by direct access or `mapGetters` method.

## How do you dispatch actions?

We can `mapActions` or call `this.store.dispatch('action name')`.

## What are the principles enforced by vuex?

1. Single source of truth
2. Data is readonly
3. Mutations are always synchronous

## What is vue router and their features?

Vue Router provides interface over web application routing for Vue instance. It allows to define routes, handle transitions and execute code on route hooks.

## What are the steps to use vue router and give an example?

In order to use Vue Router we need to create an instance of Vue Router and provide it to Vue instance. When creating vue router instance we need to pass routes declaration.

```js
// in router.js
const router = new VueRouter({
    routes: [
        {
            path: '/',
            name: 'index',
            component: SomeVueComponent
        }
    ]
})

// in main.js
const app = new Vue({
    router
}).$mount('#app')
```
