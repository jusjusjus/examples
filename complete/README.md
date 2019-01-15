## Yale BENG 406b Example

This is a complex example made available to the students of Yale BENG 406b
(Spring 2019). It makes use of some code from
[BioImage Suite Web ](https://github.com/bioimagesuiteweb/bisweb/)


## Setup

1. First install node.js (ideally v 10.x)
2. Then install the prerequisites using `npm` (on a MS-Windows
machine __omit `sudo`__)

        sudo npm install -g gulp mocha  eslint webpack webpack-cli rimraf 
        sudo npm install -g electron --unsafe-perm=true --allow-root
        sudo npm install -g electron-packager

3. Then install the local dependencies using (-d is for debug)

        npm install -d
        
4. Then build the application using

        gulp build
        
        
5. To test, first type:

        gulp webserver
        
    Then open your browser to 
    
        http://localhost:8080/build/web/index.html
        
    Alternatively run this as a desktop application using (from this directory)
    
        electron build/web
        
6. The gulp setup defines many tasks. (Type `gulp --tasks` to see the complete
   list)
   
* `gulp devel` -- runs a continuous build and watch process as you edit any js
  code. In this mode use the live html version
  `http://localhost:8080/web/index.html`
  
* `gulp package` -- will create an electron packaged application in
  `build/dist`
  
* `gulp eslint` -- will run the ESLint checker on all the .js files

and many many more.

  
  