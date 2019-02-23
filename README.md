# wasm-demo

This is a boilerplate / demo of WebAssembly. It uses a very simple C++ function (which takes a number as an argument and returns its square) in a wasm module, which can then be accessed & used from within the JS file. As soon as you pull it up on a localhost, the demo is ready to go; no configuration or setup necessary. 

I should mention that because compilation of the wasm module is done asynchronously, you need to be sure that you don't try to use the C++ function (called 'squarer' in the JS file) before it's available. The easiest way to avoid this (assuming all you want to do is text your .wasm instances) would be to call the function from within your browser's console. 


## Tutorial
(https://medium.freecodecamp.org/get-started-with-webassembly-using-only-14-lines-of-javascript-b37b6aaca1e4)

## Usage
* `npm install -g serve`
* Run command `serve` to serve `index.html`
  * Open `index.html` without `serve` will not work
* Go to `http://localhost:5000` (`index.html`)
* Open `console.log`
* Use `square` function: typing `square(10)`
