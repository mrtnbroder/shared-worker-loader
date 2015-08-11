# Shared Worker loader
Shared Worker loader for Webpack

## Usage

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

``` javascript
var MySharedWorker = require("sharedworker!./file.js");

var worker = new MySharedWorker();
worker.postMessage({a: 1});
worker.onmessage = function(event) {...};
worker.addEventListener("message", function(event) {...});
```

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
