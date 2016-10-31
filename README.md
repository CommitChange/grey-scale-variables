# grey-scale-variables

includes [precss](https://www.npmjs.com/package/precss) variables of grey-scale values:
sfasdf
```css
$grey-1: color(black l(98%));
$grey-2: color(black l(96%));
$grey-3: color(black l(92%));
$grey-4: color(black l(86%));
$grey-5: color(black l(60%));
$grey-5: color(black l(50%));

$scrim-1: rgba(0,0,0,.08);
$scrim-2: rgba(0,0,0,.5);
$scrim-3: rgba(0,0,0,.7);
```


asdf

module.exports = {
  use: [
    'postcss-import'
  , 'precss'
  , 'postcss-color-function'
  , 'autoprefixer']
, 'local-plugins' : true
, 'autoprefixers' : {browsers: 'last 2'}
, input: 'example/index.css'
, output: 'example/build.css'
}