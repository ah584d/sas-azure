This repository is about how to programmatically generate a Shared Access Signature (SAS) token to use with Postman in order to post messages to Azure Service Bus Topic/Queue.


 ## Azure SAS token generator
The current project is about how to programmatically generate a Shared Access Signature (SAS) token to use with Postman in order to post messages to Azure Service Bus Topic/Queue.

## Motivation
After googling for a while in order to generate the necessary token, to post messages to Azure service bus, i noticed that there is no clear explanations, how to ahieve it in JavaScript!!
I'm proud to offer you a simple JS way to generate Azure SAS token - using node - or angular.
## Build status
Build status of continus integration i.e. travis, appveyor etc. Ex. - 

## Code style
If you're using any code style like xo, standard etc. That will help others while contributing to your project. Ex. -

[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/feross/standard)
 
## Screenshots
Include logo/demo screenshot etc.

## Tech/framework used
Ex. -

<b>Built with</b>
- [Electron](https://electron.atom.io)

## Features
It contains two folders:
 - nodeJS: a simple node application to generate a token using your IDE
 - angular: an angular form allowing to generate a token based on the parameters filled in.

 If you prefer a simplier way to get fastly a token, you could use my angular application azure-sas-token from here:
 https://ah584d.github.io/azure-sas-token/

 This is the same application of the 'angular' folder.

 Don't forget to let me a Start :-)

## Code Example
Show what the library does as concisely as possible, developers should be able to figure out **how** your project solves their problem by looking at the code example. Make sure the API you are showing off is obvious, and that your code is short and concise.

## Installation
Provide step by step series of examples and explanations about how to get a development env running.

For node
```sh
npm install utf8
```

For angular
```sh
cd azure-sas-toekn/angular
npm install d
```
## Example (Optional)

```javascript
// code away!

let generateProject = project => {
  let code = [];
  for (let js = 0; js < project.length; js++) {
    code.push(js);
  }
};
```

## API Reference

Depending on the size of the project, if it is small and simple enough the reference docs can be added to the README. For medium size to larger projects it is important to at least provide a link to where the API reference docs live.

## Tests
Describe and show how to run the tests with code examples.

## How to use?
If people like your project they’ll want to learn how they can use it. To do so include step by step guide to use your project.

## Contribute

Feel free to open PR.

## Credits
Give proper credits. This could be a link to any repo which inspired you to build this project, any blogposts or links to people who contrbuted in this project. 

## License
A short snippet describing the license (MIT, Apache etc)

MIT © [Avraham Hamu]()
