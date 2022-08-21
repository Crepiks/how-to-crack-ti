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

Methods which modify initial array and trigger updates of view.

## What is the purpose of v-for directive?

To render list of elements according to data from interable.

## What is vuex?

Is is a global store of Vue.

## What are vuex getters?

Functions which output and (usually) transform state state.

## What are vuex mutations?

Synchronous functions which modify state.

## How do you perform mutations in components?

By calling `store.commit('name of the mutation')`.

## What are vuex actions?

Actions are functions which call mutations. Actions can be asynchronous when mutations should always be synchronous.

## Give an example usage of actions?

Actions for loading posts which call HTTP request and passes result into mutation.

## What are modules in vuex?

Modules are grouped set of actions, mutations, state and getters with specific namespace.

## How do you represent one way data flow in vuex?

Actions are called from components. Actions always call mutations. Mutations change state. State is retrieved through getters by components.

## How do you display store state in vue components?

We can access state through `mapState` or `this.store.state`. Also, state data can be retrieved through getters.

## How do you dispatch actions?

We can `mapActions` or call `this.store.dispatch('action name')`.

## What are the principles enforced by vuex?

1. Single source of truth
2. Data is readonly
3. Mutations are always synchronous

## What is vue router and their features?

Vue Router provides interface over web application routing for Vue instance. It allows to define routes, handle transitions and execute code on route hooks.

## What are the steps to use vue router and give an example?

In order to use Vue Router we need to create an instance of Vue Router and provide it to Vue instance.
