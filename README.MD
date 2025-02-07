# GSQL - a language grammar for highlight.js

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js.  You'll use the minified version found in the `dist` directory.  This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/gsql.min.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlight.js');
var hljsGSQL = require('highlightjs-gsql');

hljs.registerLanguage("gsql", hljsGSQL);
hljs.highlightAll();
```


### Author

Dan Barkus <daniel.barkus@tigergraph.com>

### Maintainer

Dan Barkus <daniel.barkus@tigergraph.com>


## Links

- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>
- Learn more about TigerGraph GSQL: <https://docs.tigergraph.com/start/gsql-101>