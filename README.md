### About

I decided I wanted to learn how to use React. This is [tic tac toe](https://facebook.github.io/react/tutorial/tutorial.html) in React. Joy.

### Notes

To compile to the browser:

    browserify -t [ babelify --presets [ react ] ] src/tic-tac-toe.jsx -o dist/tic-tac-toe.js
    
You need `browserify` globally and `babelify` plus `babel-preset-react` locally.

The React code itself requires `react` and `react-dom`.

I got this crazy `browserify` instruction out of [this tutorial](https://codeutopia.net/blog/2016/01/25/getting-started-with-npm-and-browserify-in-a-react-project/). The included tic-tac-toe example includes no details on how to get their minimum working example working...sigh...

### More notes

* The script goes *after* the main body tag on the HTML page.
* JSX is a cute macro-language.
* State is managed all at once with a `this.setState`. Elements have `props` for managing properties and `state` for managing state.
* Components should only pass state in one direction, down.
* A component dependent on a parent component is stateless.
* Explicitly write immutable code, because React determines when to redraw by checking for changes in immutable object state (this is far easier and more efficient at compile time than checking if a mutable object has changed).
* Components implementing this sort of immutability are pure components.
* cf. `immutable.js`
* Stateless components with only a `render` method are known as stateless functional components and can be written using a different, simpler syntax (which I'm going to avoid using for the moment, too much sugar).
