# Check billboard.js sideEffects on CSS

first,
```
npm install
``` 

then build.
 
```
npm run build
```

you will see `dist/main.js` only.

but if you remove `"sideEffect": false` on `node_modules/billboard.js/package.json`
or change to `["dist/**/*.css"]` then build again,

you will see not only js file but also `dist/main.css`.
