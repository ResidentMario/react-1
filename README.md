### About

I decided I wanted to learn how to use React. This is [tic tac toe](https://facebook.github.io/react/tutorial/tutorial.html) in React. Joy.

### Notes

To compile to the browser:

    browserify -t [ babelify --presets [ react ] ] src/tic-tac-toe.jsx -o dist/tic-tac-toe.js
    
You need `browserify` globally and `babelify` plus `babel-preset-react` locally.

The React code itself requires `react` and `react-dom`.

I got this crazy `browserify` instruction out of [this tutorial](https://codeutopia.net/blog/2016/01/25/getting-started-with-npm-and-browserify-in-a-react-project/). The included tic-tac-toe example includes no details on how to get their minimum working example working...sigh...