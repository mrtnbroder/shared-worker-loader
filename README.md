# Shared Worker loader

Shared Worker loader for Webpack.

## Usage

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

``` javascript
var MySharedWorker = require('shared-worker!./file.js')

var worker = new MySharedWorker()
worker.addEventListener('message', (e) => {...})
worker.port.onmessage = (e) => {...}
worker.port.start()
```

## Credits

Thanks [@sokra](https://github.com/sokra) for providing the codebase found within [worker-loader](https://github.com/webpack/worker-loader)!

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
