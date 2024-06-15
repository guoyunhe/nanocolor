# fastcolor

Color class 2~4x faster than `@ctrl/cinycolor`. Can be a drop-in replacement for `@ctrl/tinycolor`, with the follwing differences:

- Don't support CSS color names, like `'darkgreen'`, `'orange'`. This helps reduce bundle size.
- Don't support CMYK, HSL, HSV as input and output formats. This helps reduce bundle size and improve performance.

```
npm install --save fastcolor
```

```js
import { FastColor } from 'fastcolor';

new FastColor('#66ccff');
new FastColor('rgba(102, 204, 255, .5)');
```

## TODO

- darken()
- isLight()
- lighten()
- onBackground()
- setAlpha()
- toHexString()
- toHsl().l
- toRgb()
- toRgbString()
