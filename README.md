# Javascript REPL

Javascript REPL is a javascript playground for Visual Studio Code with live feedback(logs or errors) as you type, besides your code, in a log explorer, or in an output channel. It supports Javascript, TypeScript, CoffeeScript and it can be used for development in Node.js projects or with frond end frameworks like React, Vue, Angular, Svelte etc.

![Screenshot of vscode javascript repl with react project](./preview1.png)

## Features

By pressing cmd(or ctrl) + shift + l as shortcut or by using the command "JS Repl: Run" and by using console.log statement,you can display the result of whatever expression you want (Variable, Function, Object etc..). JS Repl can be activated on file types(.js, .ts, .coffee, .jsx, .tsx, .vue) or by launching "JS Repl: New ..." available commands.

- Logs through comments or by using console.log
- Show or copy value of an expression, without add comments or console.logs
- Logs explorer at the left
- Output window with all the logs
- Live code coverage
- Imported files support
- Easy install for missing modules
- Multi files loggins or errors per project
- async results rendering
- JavaScript, TypeScript and CoffeeScript support

![Screenshot of vscode javascript repl with Vue project](./preview2.png)

### Logging

Users can add logs in their code with the following ways:

```js
// You can add logs by using console.log
console.log('We ♡ JavaScript!');

// or by using a comment line with equals sign at the end of an expression
const obj = {
  language: 'javascript'
}; //=

function hello() {
  return 'Hello World!';
}
// or a comment block with equals sign
hello(); /*= */

// or just type the variable name
obj;

// if the log represents an object you can use the dollar sign to access its properties
obj; //= $.language

//  also inside the log comments you can print every expression in your scope
hello(); //= obj

// Besides, you can select one or more variables or expressions and press right click
//and select show value or explore the logs at the explorer on the left
```

## Credits

The icons that I used are not mine, so I would like to say thank you to the following sources or persons:

- [Flaticon](https://www.flaticon.com/authors/freepik)
- [Dave Gandy on flaticon](https://www.flaticon.com/authors/dave-gandy)
- [Vaaddin on flaticon](https://www.flaticon.com/authors/vaadin)
- [Font Awesome](https://fontawesome.com/)

This extension uses under the hood a modified version of [Parcel](https://parceljs.org/) bundler. So I would like to say a big thank you to the guys there. You can find the modified version at the following [branch](https://github.com/axilleasiv/parcel/tree/vs-repl).

## Inspiration

I'd like to give a shout out to [Quokka.js](https://quokkajs.com), which is a significantly more comprehensive and covers a lot more editors, if this extension interests you - check out that too. Also, when I started to play around this, I started with the code of the following [extension](https://github.com/lostfields/vscode-nodejs-repl)
