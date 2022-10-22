# SystemJS Example

1. Run `http-server`
2. Load http://127.0.0.1:8080 in a broser
3. Open Chrome DevTools
4. Click both buttons

## Errors & Fixes

|Error|Fix|
|-|-|
`Uncaught SyntaxError: Cannot use import statement outside a module` or `Uncaught SyntaxError: Unexpected token 'export'` | Use systemjs-babel
systemjs-babel error: `Invalid regular expression:`| Solution: Included `<meta charset="utf-8">` in the `<head>` tags of the HTML document. Reference: https://github.com/babel/babel/issues/340#issuecomment-113982116
`Access to fetch at 'file:///.../node_modules/garretts-dogs/index.js' from origin 'null' has been blocked by CORS policy: Cross origin requests are only supported for protocol schemes: http, data, isolated-app, chrome-extension, chrome, https, chrome-untrusted.` | A server is necessary to load local files. Use https://www.npmjs.com/package/http-server - i.e. run http-server from project directory to run your application on a static HTTP server.
