<img src="pictures/icon.svg" align="right" />

## Azure SAS token generator
> A simple JavaScript Azure SAS token generator


The current project is about how to programmatically generate a Shared Access Signature (SAS) token to use with <a href="https://github.com/ah584d/azure-send-message-to-service-bus-with-postman">Postman in order to post messages to Azure Service Bus Topic/Queue.</a>

![NPM](https://img.shields.io/npm/l/azure-sas-token) ![GitHub issues](https://img.shields.io/github/issues-raw/ah584d/azure-sas-token) ![Snyk Vulnerabilities for npm package](https://img.shields.io/snyk/vulnerabilities/npm/azure-sas-token) ![npm](https://img.shields.io/npm/v/azure-sas-token) ![npm bundle size](https://img.shields.io/bundlephobia/minzip/azure-sas-token) ![npm bundle size](https://img.shields.io/bundlephobia/min/azure-sas-token) ![npm](https://img.shields.io/npm/dt/azure-sas-token)
## Motivation
After googling for a while in order to generate the necessary token, to post messages to Azure service bus, i noticed that there is no clear explanations, how to achieve it in JavaScript!!
I'm proud to offer you a simple JS way to generate Azure SAS token - using node - or angular.

## Features
It contains two folders:
 - nodeJS: a simple node application to generate a token using your IDE
 - angular: an angular form allowing to generate a token based on the parameters filled in.

If you prefer a simplier way to get fastly a token, you could use my angular application azure-sas-token from here:
https://ah584d.github.io/azure-sas-token/

This is the same application of the 'angular' folder.

Don't forget to let me a Star &#11088; :-)
 
## How to use?
[angular version]: you can use the online version, or to checkout the repository and run it locally on your computer

[node version]: only by adding the dependency to your code, see example section

## Screenshots
The application is totally safe, nothing is saved on third party, no request is sent outside, everything is handled in JS browser side
![Azure SAS token generator](https://github.com/ah584d/azure-sas-token/blob/master/pictures/sas.jpg)

For those who still hesitate, you can checkout the code and run it locally on your computer

```sh
npm run start
```

## Installation

For node
```sh
npm install azure-sas-token
```

For angular
```sh
cd azure-sas-token/angular
npm install

POST https://<yournamespace>.servicebus.windows.net/<yourentity>/messages
Content-Type: application/json
Authorization: SharedAccessSignature sr=https%3A%2F%2F<yournamespace>.servicebus.windows.net%2F<yourentity>&sig=<your token generated by this repository code>&se=1438205742&skn=KeyName
```

## Code Example
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/feross/standard)
```javascript
For node:

const createSharedAccessToken = require('azure-sas-token').default;

const sasToken = createSharedAccessToken('https://<service namespace>.servicebus.windows.net/<topic name or queue>',
								'<signature key name>',
								'<signature hash>');

console.log(`sasToken: ${sasToken}`);
```

## Posting messages in Azure service-bus queue - tutorial
https://github.com/ah584d/azure-send-message-to-service-bus-with-postman

## Tests
On going...

## Build status [under construction]

## Contribute
Feel free to open PR.

## Credits
The only related topic that I founded on Microsoft Azure help

https://docs.microsoft.com/en-us/rest/api/eventhub/generate-sas-token

Icon from: http://www.kameleon.pics

## License
A short snippet describing the license (MIT, Apache etc)

MIT © [Avraham Hamu]()
