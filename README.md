# highlightjs-codeowners

## Description

codeowners - a language grammar for highlightjs

## Usage

Include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js. You'll use the minified version found in the `dist` directory. This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" charset="UTF-8"
  src="/path/to/highlightjs-codeowners/dist/codeowners.min.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```

### Using directly from the UNPKG CDN

```html
<script type="text/javascript"
  src="https://unpkg.com/highlightjs-codeowners/dist/ccodeowners.min.js"></script>
```

- More info: <https://unpkg.com>

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlightjs');
var hljsCodeowners = require('highlightjs-codeowners');

hljs.registerLanguage("codeowners", hljsCodeowners);
hljs.highlightAll();
```