# metalsmith-org

A [Metalsmith][1] plugin to convert org-mode files.

## Installation

```
npm install metalsmith-org
```

## CLI Usage

Install via npm and then add the `metalsmith-org` key to your `metalsmith.json` plugins with any [org-js][2] options you want, like so:

``` js
{
  "plugins": {
    "metalsmith-org": {
      "headerOffset": 1
    }
  }
}
```

## Javascript Usage

Pass `options` to the org plugin and pass it to Metalsmith with the `use` method. `metalsmith-org` does not have any options of its own, everything here will be passed on to [org-js][2]:

``` js
var org = require('metalsmith-org');

metalsmith.use(org({
    headerOffset: 1
}));
```

## License

MIT

[1]: http://metalsmith.io "Metalsmith static site generator"
[2]: https://github.com/mooz/org-js.git "org-js"
