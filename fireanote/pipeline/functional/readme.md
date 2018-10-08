# Node.js testing #

## How to install the project ##
Install node.js and upgrade to the latest
* npm install -g npm@latest

Install packages
* npm install [yo](http://yeoman.io)
* npm install [generator-protractor](https://www.npmjs.com/package/generator-protractor)
* npm install [protractor](https://www.protractortest.org/)
* npm install [chai](https://www.chaijs.com/)

## Structure ##
package-json<br/>
List of project dependencies<br/>
|- node_modules<br/>
Locally installed packages not to be included in the SCM<br/>
|- spec<br/>
Test/specs go in the spec directory.<br/>

The [protractor configuration](protractor.conf.js) points to the tests.

## How to run the tests ##
If using local installs then create a couple of batch/shell files to start [webdriver-manager](webdriver-manager.bat) and [protractor](protractor.bat).

1. Start the Selenium server: 
`webdriver-manager start`

2. Open a new terminal and run Protractor: 
`protractor protractor.conf.js`

# References #
Protractor tutorial - [Tutorial](https://www.protractortest.org/#/tutorial)<br/>
BDD - [BDD made simple in Node.JS with Mocha and Chai](https://itnext.io/bdd-made-simple-in-node-js-with-mocha-and-chai-3a3ce44ecce2)<br/>
A Yeoman code generator for Protractor - [generator-protractor](https://github.com/andresdominguez/generator-protractor)<br/>

