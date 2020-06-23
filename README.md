# QUX-LowCode
Quant-UX (http://www.quant-ux.com) is an OpenSource UX tool for the design and test of user interfaces. The QUX-LowCode package
provides a new approach to the hand-off problem (See details below). The core of the solution is the QUX component,
which renders the visual design and allows the developers to focus on business logic, without restricting the developers' freedom. The component enables:

1. Zero Code rendering of visual design and animations
2. Clear separation of UI and business logic
3. Developers can focus on code
4. Developers can use the tools and frameworks of their choice.
5. Designers can use the powerful visual design tool
6. Easy extension with custom callback functions
7. Full support of VUE data binding.
8. Extension with custom components
9. Extension with custom CSS
10. Rich library of stylable components.

## The handoff problem
Designers and developers use different tools to build user interfaces. Once a designer has completed the interface design, he hands-off the design to the developer, usually in the form of an image and some specs.
The developer has now to rebuild the entire design using the programming language of his choice.
Although this process is proven, it is rather slow and not very efficient. In particular later changes in
the design makes it hard to automize this work through code generation tools.

## Envisioned workflow

We envision the following workflow to enable painless collaboration between designers and developers:

![The QUX low code workflow](assets/Workflow.png "QUX LowCode workflow")

1. The designer creates an initial design in Quant-UX
2. The developer adds data binding and method callbacks in Quant-UX using a dedicated view.
3. The developer sets up a new project (Vue.js for now) and includes the QUX component
4. The developer loads the design from Quant-UX and creates the required methods and fills them with business logic.
5. The QUX component renders the design and invokes the callbacks in clicks.
6. Changes in the design are transparent to the developer, he just reloads the design from Quant-UX.


# How to use qux-lowcode

First, you have to install the QUX-LowCode package via NPM

```
npm i react-native-low-code
```


```
npm install
```

Build:
```
npx bili --bundle-node-modules
```