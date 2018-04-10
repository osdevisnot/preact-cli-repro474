# preact material app

## Observations

* create project using command: `preact create material preact-cli-repro474`
* run in prod mode using: `npm run serve`

* 1st run - load https://localhost:8080 in browser
  ![Image for 1st run](docs/run01.png?raw=true 'Title')

* 2nd run - just reload the browser
  ![Image for 2nd run](docs/run02.png?raw=true 'Title')
* change src/route/profile/index.js

* 3rd run - run `npm run serve` and reload browser after `npm run serve` is complete
  ![Image for 3rd run](docs/run03.png?raw=true 'Title')
* Note differences in sw.js between 2 runs:

```js
var precacheConfig = [
  ['/bundle.8f843.js', '7df369715fe18248f9c0c1c10ef6787c'],
  ['/index.html', 'b5de0ffd79cb85001089543d7543365d'],
  ['/route-profile.chunk.473c0.js', '1e8a0d3d18b9c6c9d4f84ffaab54c144']
];

var precacheConfig = [
  ['/bundle.2029a.js', 'c46db1dbf4d59ba075d2d9aafe49d38c'],
  ['/index.html', '0906d1b1e7ad5c209a5e3b293e409704'],
  ['/route-profile.chunk.c96cb.js', 'ebd8756d29665031bbd7e16b2c385d0f']
];
```

* 4th run - just reload the browser
  ![Image for 4th run](docs/run04.png?raw=true 'Title')
