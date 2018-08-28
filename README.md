# Expressions Unit Test Library
A small environment which allows to add unit tests to expressions.

## How to prepare:
### Prepare the repository
- Install [npm](https://www.npmjs.com/get-npm)
- ```git clone <this respository>```
- Install dependecies with ```npm install```

### Add your code
- If your customization area is under version control, clone it to the folder ```customizationArea``` with ```git clone <repository> customizationArea```
- If your customization area is not under version control, copy it into the folder ```customizationArea```


- If you want to paste in your expressions directly from the Product Editor, you have to paste them into the file located at `customizationArea/integration/externalProduct/customJSFunctions.js` and put it into a named function

#### Example
 Your expression:
 ```tag("$red")```

 Put it into the `customJSFunctions.js` like this:
 ```
 function myFunction(){
   tag("$red")
 }
 ```
Then you can use the function in the test file as myFunction()
- This library reads the file `customJSFunctions.js` from ```customizationArea/integration/externalProduct/customJSFunctions.js```. You can change that path in the `config.json`

## How to write tests:
- This framework is based on  [jest](https://jestjs.io).
- Use our [example repository](https://github.com/OpusCapita/pim-integrations-expression-unit-test-examples) for in-depth examples and documentation.
- All functions usually available within an expression, like `term` and `boilerplate`, are set up as [jest-mocks](https://jestjs.io/docs/en/mock-functions). See the example repository for details.

## How to use
- Type `npm start` to run the tests

## Notes
- This test suite does not support ES6 features in expressions.
- This test suite does currently not support the `format` functions from PIM.

## Compatibility
- This test suite works with PIM 8.10m1


## Contributing
We are happy to accept pull requests.

## Contributors

| [<img src="https://avatars.githubusercontent.com/u/41996712" width="100px;"/>](https://github.com/uwestolz) | [**Uwe Stolz**](https://github.com/uwestolz)     |
| :---: | :---: |
| [<img src="https://avatars.githubusercontent.com/u/36043138" width="100px;"/>](https://github.com/davidbrien) | [**David Brien**](https://github.com/davidbrien)     |
| [<img src="https://avatars.githubusercontent.com/u/30691117" width="100px;"/>](https://github.com/alexejFroebel) | [**Alexej Froebel**](https://github.com/alexejFroebel)     |
 [<img src="https://avatars.githubusercontent.com/u/4085533" width="100px;"/>](https://github.com/pflenker) | [**Philipp Flenker**](https://github.com/pflenker) |
