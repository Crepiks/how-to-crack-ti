# Vue Interview Answers

## What is VueJS?

VueJS is a client side JavaScript framework which allows developers to be more performant when developing web applications.

## What is the difference between v-show and v-if directives?

`v-show` adds `display: none` CSS attribute to the element so that element disapears from web page but remains present in DOM. `v-if` completely removes element from DOM.

## Why do you need to use key attribute on for directive?

`key` attribute is used to uniquely indentify element in the list and to present unnecessary rebuilding.

## What are props?

Props is a reactive data passing into component.

## How do you communicate from child to parent using events?

By emitting events and passing data in second argument.

## How do you implement model on custom input components?

By using `model` param and specifing input prop and output event.

## What are slots?

Slots are markups passed in inside the tags into component.

## What are mixins?

Mixins is a code which can be added into component.

## What is scoped CSS?

Scoped CSS is a styles which are applied to specific component and its children.

## Why the component data must be a function?

Component data is a function to prevent sharing data among all instances of the component.

## What are the lifecycle methods of VueJS?

`beforeCreate`, `created`, `beforeMount`, `mounted`, `beforeUpdate`, `updated`, `beforeUnmount` and `unmounted`.

## What is vue instance?

Is an instance of Vue application with scoped global context, components, store and so on.

## What are the conditional directives?

Conditional directives are directives used to conditionaly render or display elements.

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
