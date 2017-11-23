## React Manual
> คู่มือการใช้งาน React

## Table of Contents
- [JSX](#jsx)
- [Babel](#babel)
- [Webpack](#webpack)
- Rendering Elements
- Components and Props
- State and Lifecycle
- Handling Events
- Conditional Rendering
- Lists And Keys
- Forms
- Lifting State Up
- Composition vs Inheritance
- JSX In Depth
- Typechecking with PropTypes
- Static Type Checking
- Refs and The DOM
- Uncontrolled Components
- Optimizing Performance
- React Without ES6
- React Without JSX
- Higher-order Components
- Integration with Other Libraries
  - Router
  - Redux
- Tests
- Server Side Rendering

## JSX
> Javascript XML

public\index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>
  <div id="app"></div>
  <script src="https://unpkg.com/react@16.0.0/umd/react.development.js"></script>
  <script src="https://unpkg.com/react-dom@16.0.0/umd/react-dom.development.js"></script>
  <script src="/scripts/app.js"></script>
</body>
</html>
```

public/app.js
```javascript
var template = React.createElement(
  "h1",
  { id: "someid" },
  "Hello JSX!"
);

ReactDOM.render(template, document.getElementById('app'));
```

## Babel
- Shell
> npm install --save-dev babel-loader babel-core

- Via config
```javascript
module: {
  rules: [
    { test: /\.js$/, exclude: /node_modules/, loader: "babel-loader" }
  ]
}
```
- Create .babelrc configuration file
  - Shell
    > npm install babel-preset-env --save-dev
  - .babelrc
    ```javascript
    {
      "presets": ["env"]
    }
    ```
- Plugin React
  - Shell
    > npm install --save-dev babel-cli babel-preset-react
  - .babelrc
    ```javascript
    {
      "presets": ["react"]
    }
    ```
## Webpack
คู่มือการใช้งาน [Webpack](https://github.com/yuttasakcom/WebpackManual) ฉบับ YoProgrammer

