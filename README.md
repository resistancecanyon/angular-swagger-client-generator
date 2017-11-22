# angular-swagger-client-generator
Angular API client generator from Swagger JSON specification

# Description
This package generates a Angular 4 TypeScript classes from a Swagger v2.0 specification file. The code is generated using Mustache templates.

The generated service class uses new [HttpClient](https://angular.io/guide/http) module of Angular 4.

# How to get it working

## Installation

`npm install angular-swagger-client-generator`

or  

`git clone https://github.com/resistancecanyon/angular-swagger-client-generator`  
`cd angular-swagger-client-generator`  
`npm install`  
`npm run build`  

## Usage

From command line, run:
```
a4apigen -s [yopur/path/to/swagger.json]
```

or
```
a4apigen -u [url/of/your/swagger.json]
```

## Example usage:

This command will generate API client described in swagger.json file to ./out folder
```
a4apigen -s ./tests/apis/swagger.json -o ./out
```

or from repository directory run:
```
node ./src/a4apigen -s ./tests/apis/swagger.json -o ./out
```

## Note:
This project was inspired by [swagger-js-codegen](https://github.com/wcandillon/swagger-js-codegen) project.
