# OPEND_NSWBirthRate

- This OPEND subproject deals with NSW residential population from different NSW suburbs. 

- Data was obtained from:
[http://www.abs.gov.au/ausstats/abs@.nsf/DetailsPage/2033.0.55.0012011?OpenDocument](http://www.abs.gov.au/ausstats/abs@.nsf/DetailsPage/2033.0.55.0012011?OpenDocument)
  - .xls file: State Suburb, Indexes, SEIFA 2011 (2033.0.55.001 ssc indexes.xls / table 2)


- This work is licensed under https://creativecommons.org/licenses/by/4.0/

## development process:
- install node
  - then we can use npm 
- install bower
  - run: 
    ``` 
    npm install -g bower 
    ```
- using bower
  - make directory static, and enter directory static
  - add bower.json
  - run: 
    ```
    bower install
    ``` 
    to install required front-end packages. directory bower_components is created.

- using babel 
  - run 
    ```
    npm install --save-dev babel-cli babel-preset-env babel-preset-react
    ```
    to install babel-cli, babel-preset-env, babel-preset-react. directory node_modules is created.


  - add .babelrc
  - run:
    ```
    babel js/ --out-dir lib/
    ```
    to compile javascript codes.
  - (if we run: 
  ```
  babel js/ --out-dir lib/ --watch
  ```
    babel will keep running and compile modified file automatically)
    
    
- using require.js

  - add build.js
  - download r.js from <http://requirejs.org/docs/download.html>
  - run 
  ```
  node r.js -o build.js
  ```
  - index.html uses the file packaged by require.js. index_debug.html uses files before packaged by require.js. 
  


