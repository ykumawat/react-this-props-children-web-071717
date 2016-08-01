# React this.props.children

## Objectives

1. Explain what `this.props.children` means in the context of a React component
2. Explain how to use the `React.Children` utilities
3. Practice using and iterating over child components

## Overview

I suspect that this lab will prove a bit more challenging than the other ones in
this unit. We first want students to understand that `this.props.children` just
refers to any components passed in as children.

A good way to demonstrate this is with a page layout component, e.g.,

```
class Layout extends Component {
  render() {
    return (
      <div>
        <header style={{ ... }}>Header; maybe some links</header>
        {this.props.children}
        <footer style={{ ... }}>Footer</footer>
      </div>
    )
  }
}
```

Have students practice writing and rendering a component like this with
different child components. Make sure to have at least one example that uses
an array of siblings as `this.props.children`.

Then start walking through the `React.Children` API. These methods should be
easy to understand once students have a grip on how `this.props.children` works.


## Resources

- [React.Children](https://facebook.github.io/react/docs/top-level-api.html#react.children)
