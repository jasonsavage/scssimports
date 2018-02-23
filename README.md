# scssimports
npm script that tries to mimic what gulp-sass-bulk-import does


## Example

Add the following code to the scrips section of your package.json file:

```json
// package.json
{
	"scripts": {
		"scssimports": "node scripts/scssimports.js \"../src/assets/scss/main.scss.tpl\""
	}
}
```

example main.scss.tpl file

```scss
// main.scss.tpl
//components
@import "components/*";

// application
@import "application/*";
```

> **NOTE:** this is a pretty basic implementation so the glob pattern seen in main.scss.tpl does't fully work
