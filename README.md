# JSON3 is JSON

This is a hack for 3rd party libraries that have json3 as a dependency. This simply replaces JSON3 with nativ JSON.

## Installation

Add `"json3": "github:footageone/fake-json3"` to your `package.json`

Add resolution to github to your package.json

```
"resolutions": {
    "json3": "github:footageone/fake-json3"
  },
```

And `"preinstall": "npx npm-force-resolutions"` to your scripts section.

This will replace json3 with native json for libraries that require json3 as a library
