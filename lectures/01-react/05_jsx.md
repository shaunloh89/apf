
### Wait - What's that HTML doing in my Javascript?

This is currently the contents of our `app.js` file:

```js
// bring in React and Component from React

import React, {Component} from 'react'

// define our Hello component
class Hello extends Component {
  // what should the component render?
  render () {
    // make sure to return some UI
    return (
      <h1>Hello World!</h1>
    )
  }
}

export default Hello
```

Let's talk about the value that the `render` method returns. It looks an awful lot like an HTML header, but it's not. Often times we write out React components in **JSX**.

Wait, what's that? Try it yourself alongside this video in [this codepen](https://codepen.io/susir/pen/wJPoBw).

<iframe src="//fast.wistia.net/embed/iframe/dcps4dqziy?seo=false" title="Wistia video player" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" allowfullscreen mozallowfullscreen webkitallowfullscreen oallowfullscreen msallowfullscreen width="640" height="360"></iframe>


So, JSX allows us to write code that strongly resembles HTML. It is eventually compiled to lightweight JavaScript objects. We're returning some JSX that creates a header with 'Hello World' in it for our component to render.

> React can be written without JSX. We won't be doing this, but if you want to learn more, [check out this blog post](http://jamesknelson.com/learn-raw-react-no-jsx-flux-es6-webpack/). This link is also in the Further Reading page at the end of the React module.

### Challenge: Greet the day!

In your component, return multiple lines. Instead of just the "Hello World!" header, also add a line below it that will display `"It is time for tea."` in an `h3`.

> Hint: Remember, the return statement in `render` can only return one DOM element. You can, however, place multiple elements within a parent `div` element.*

You can check your solution [here](https://git.generalassemb.ly/education-product/module-fe-framework-react/tree/master/exercise-solutions/jsx-hello-world).
