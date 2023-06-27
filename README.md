## React Workshop Teaching Demo Lesson Plan

### Starter Code - [Here](https://codesandbox.io/s/react-state-demo-starter-8vmckv?file=/src/App.tsx)
- Review the starter code provided, which includes a basic React application with TypeScript.
- Note the `Button` component, defined with TypeScript interfaces and the `React.FC` (Function Component) type. It receives `text` for button content and `onClick` function as props.
- Note the `Counter` component that uses the `Button` component, with a number display `0` and a button that triggers a `console.log`.

---

### Introduction to State in React [Here](https://codesandbox.io/s/react-state-demo-starter-objective-1-vxgykc?file=/src/App.tsx:0-676)
- Learning Objective:  Understand the concept of state in React, introduced with the `useState` hook.
- Note the usage of `useState` in the `Counter` component, where the `count` state variable is initially set to `0`.
- Notice how `count` replaces the hard-coded `0` in the `Counter` component.
- The `handleClick` function, which replaced the `console.log` statement in the `Button`'s `onClick` prop,  updates `count` state.

---

### Handling Click Events in React [Here](https://codesandbox.io/s/react-state-demo-starter-objective-2-r2k5wm?file=/src/App.tsx:0-705)
- Learning Objective:  Understand how to handle click events in React and how to call a function with an argument in an event handler.
- The updated `handleClick` function in the `Counter` component, which takes a number as an argument, increases `count` by this given number.
- Note that how `handleClick` is passed to `Button`'s `onClick` as an arrow function which calls `handleClick` with `2` as an argument.

---

### Moving State Up the Component Tree [Here](https://codesandbox.io/s/react-state-demo-starter-objective-3-pgtr92?file=/src/App.tsx:0-1130)
- Learning Objective: Understand the concept of lifting state up when it needs to be shared among multiple components.
- Observe how `countOne` and `countTwo` state variables have been moved to the `App` component.
- Note also that there are now multiple `handle` functions to update `countOne` and `countTwo`.
- The `Counter` components now take `count` and `handleClick` as props, and each `Counter` has its own `count` and `handleClick` to handle the seperate logic.
- Now, we are able to calculate total count by adding `countOne` and `countTwo`.

---

### Project - Building a Painting Slider [Here](https://codesandbox.io/s/finished-react-state-demo-mvswxv?file=/src/App.tsx:0-1970)
- Assignment:  Build an interactive painting slider by creating a `Painting` component.
- Create a `paintings` array filled with image addresses of an artist of your choice.
- Use the `useState` hook to keep track of the current index in the `paintings` array.
- Initialize the index as `0`, and set it to increase or decrease when the "next" or "last" buttons are clicked, respectively.
- Ensure the index always stays within the bounds of the `paintings` array.
- Style the page!
