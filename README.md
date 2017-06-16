# require-polyfill

Include this module in your Karma tests to provide `require` if your module is built with CommonJS modules.

## Installation

```
npm install --save-dev require-polyfill
```

Then include it in your `karma.conf.js`:
```
module.exports = function (config) {
    'use strict';
    config.set({

        ...
        files: [
            './node_modules/require-polyfill/index.js',
            ...
        ],
        ...
    });
};
```
