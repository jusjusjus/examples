![Logo](https://bioimagesuiteweb.github.io/bisweb-manual/bisweb_newlogo_small.png)

---

# Examples Repository

This is example code for BioImage Suite Web. It introduces certain JavaScript
and Software Engineering Concepts. 

To use (parts of) BioImage Suite Web as a library you can install it via npm

For node.js

    npm install biswebnode
    
For browser/electron

    npm install biswebbrowser


---

## Learning JavaScript

These examples intoduce certains aspects of JavaScript but they are not a
complete introduction to the language.  For this the reader is referred to the
two books by Axel Rauschmayer. The first, which covers JavaScript up to
version 5 (standard usage until maybe 2016) , is
[Speaking JS](http://speakingjs.com/es5/) by Axel Rauschmayer. Part I -- "A
JavaScript QuickStart" may be all that you need to read to get
started. JavaScript v6 (ES2015) is now fast becoming the new standard. A
second book called [Exploring ES6](http://exploringjs.com/es6/index.html) by
the same author covers some of the changes. I strongly recommend reading
Chapters 1-4 for a clear understanding of all that is new here. Finally, we
recommend this
[document from the BioImageSuite Web repository](https://github.com/bioimagesuiteweb/bisweb/blob/master/docs/AspectsOfJS.md)
which highlights some aspects of the language that are particularly relevant
to these examples.

---

## Before you begin

 * Install Node.js 10.x (LTS) -- you may download this from:

    [https://nodejs.org/en/download/](https://nodejs.org/en/download/). 
    
 
 * Install the following global prerequisites using `npm` (on a MS-Windows
   machine __omit `sudo`__)

        sudo npm install -g gulp mocha jsdoc eslint modclean webpack webpack-cli uglify-es rimraf 
        sudo npm install -g electron --unsafe-perm=true --allow-root
        sudo npm install -g electron-packager
---

## Examples Of Using BioImage Suite Web as a library

The following two directories illustrate the use of the npm packages
`biswebnode` and `biswebbrowser`.

* [biswebnode](./biswebnode_examples) -- examples of using the node.js package
  `biswebnode` as a library.
  
* [biswebbrowser](./biswebbrowser_examples) -- examples of using the
  browser/electron package `biswebbrowser` as a  library.

---

## A Complete Simple Application Example in 10 Steps

This set of examples shows how to create both the code and, more critically,
the development/build environment for a multi-context (web, electron, PWA)
application. The application itself is trivial -- it simply computes the BMI
given height and weight information. The focus here is really on the software
engineering infrastructure aspects of the problem.

This set of examples was developed in part also for the needs of the Yale
Course ``Medical Software Design`` (BENG 406b, Spring 2019).


* [Step 1](./step01) -- a simple commandline (node.js)  `helloworld` application.
* [Step 2](./step02) -- a slightly more complex node.js application showing how
  to use a module.
* [Step 3](./step03) -- a simple web-based application showing how to use an
  old-fashioned module. We also introduce here `npm` and the associated
  package file `package.json` and the task runner `gulp`.
* [Step 4](./step04) -- a redo of step 3 using proper modules and the webpack
  ''bundler''. We also introduce regression testing using `mocha`.
* [Step 5](./step05) -- a redo of step 4 but now as a desktop application using
  Electron.
* [Step 6](./step06) -- moving step 5 to web-components (custom web elements)
* [Step 7](./step07) -- Using
  [BioImage Suite Web code](https://github.com/bioimagesuiteweb/bisweb) to create menus, file dialogs and file I/O
* [Step 8](./step08) -- Progressive web applications.
* [Step 9](./step09) -- packaging web applications for deployment to a web server.
* [Step 10](./step10) -- extra code for packaging electron-based desktop applications.
  distribution. 
* [Complete](./complete) -- the full example with desktop and electron and pwa
  versions. This is the boiler-plate template  for BENG 406b projects.
  

---

BioImage Suite Web (bisweb) is a web-based medical image analysis suite
primarily geared towards Neuroimaging Analysis. We gratefully acknowledge
support from the [NIH Brain Initiative](https://www.braininitiative.nih.gov/)
under grant R24 MH114805 (Papademetris X. and Scheinost D. PIs).
