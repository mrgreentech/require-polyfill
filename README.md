# require-polyfill

Include this module in your Karma tests to provide `require` if your module is built with CommonJS modules.

## Installation

```
npm install --save-dev git+ssh://git@stash.mrgreen.zone:7999/gar/require-polyfill.git#v1.0.0
```

**NOTE:** make sure that the URL sticks in your `package.json`. If you see something else than the above URL for `"require-polyfill"` replace it with the URL.

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
