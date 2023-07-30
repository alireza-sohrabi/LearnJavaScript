# JavaScript Modular programing

## In JavaScript, modules refer to a file that holds JavaScript code which performs a specific purpose.

Modules are self-contained, making it easy to add, remove, and update functionalities without affecting your entire code because they are decoupled from other pieces of code.

When you have these modules in separate JavaScript files, you'll want to use them within the original JavaScript file.

In this article, you will learn what the `require()` function does, how you can use it, and some distinct differences between the require and import functions.

For a long time, the CommonJS module system has been the default module system within the Node.js ecosystem. But a new module system was introduced in Node.js v8.5.0, which is the ES module system.

CommonJS and EMCAScript modules (ES modules) now work perfectly in Node.js. The major difference between them is their execution.


## How to Execute CommonJS and ES Modules

In the browser, JavaScript module execution depends upon `import` and `export` statements. These statements load and export ES modules, respectively. This is the standard and official way to reuse modules in JavaScript, and it’s what most web browsers natively support.

Node.js, by default, supports the CommonJS module format, which loads modules using the `require()` function, and exports them with `module.exports`.

## What is the JavaScript require() Function?

The `require()` function is straightforward to use and understand, as all you have to do is assign the function to a variable.

In this function, you will pass the location name as an argument. Here is the general syntax:

```javascript const varName = require(locationName)```


## require() vs import() Functions

The require and import functions/statements are used to include modules within your JavaScript file, but they possess some differences. The two major differences are:

- The require() function can be called from anywhere within the program, whereas import() cannot be called conditionally. It always runs at the beginning of the file.
- To include a module with the require() function, that module must be saved with a .js extension instead of .mjs when the import() statement is used.
