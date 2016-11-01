# grey-scale-variables

includes [precss](https://www.npmjs.com/package/precss) variables of grey-scale values.
intended to use with [postcss](https://github.com/postcss/postcss).

```css
$grey-1: color(black l(98%));
$grey-2: color(black l(96%));
$grey-3: color(black l(92%));
$grey-4: color(black l(86%));
$grey-5: color(black l(60%));

$scrim-1: rgba(0,0,0,.08);
$scrim-2: rgba(0,0,0,.5);
$scrim-3: rgba(0,0,0,.7);
```

### example:

package.json
```javascript
{
  "scripts": {
    "build-css": "postcss -c postcss-config.js",
    "watch-css": "postcss -c postcss-config.js -w"
   },
  "devDependencies": {
    "postcss",
    "postcss-cli",
    "postcss-import",
    "precss",
    "postcss-color-function",
    "@commitchange/grey-scale-variables"
  }
  etc...
}
```

postcss-config.js
```javascript
module.exports = {
  use: ['postcss-import', 'precss', 'postcss-color-function']
, 'local-plugins' : true
, input: 'index.css'
, output: 'build.css'
}
```

index.css
```css
@import '@commitchange/grey-scale-variables';

body {
	background: $grey-1;
}

```

```
npm run watch-css
```
