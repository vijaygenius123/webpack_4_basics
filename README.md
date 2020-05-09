# webpack_4_basics


## Create A Basic Structure

directory structure with files like below
```bash
dist/
    index.html
src/
    index.js
.gitignore
package.json
```

## Install Webpack , Webpack-Cli And JQuery


Added below content to dist/index.html
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Webpack Basics</title>
</head>

<body>
    <h1 id="target">Hello World</h1>

    <script src="main.js"></script>
</body>

</html>
```

Added below code to src/index.js
```js
const $ = require('jquery')

setTimeout(function () {
    $('#target').text("Hello Webpack")
}, 1000);
```

and ran
```bash
.node_modules/.bin/webpack
```

This will run webpack with default configuration