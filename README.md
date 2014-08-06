# gulp-uglify-inline

gulp-uglify-inline is a [gulp](https://github.com/wearefractal/gulp) plugin to uglify inline scripts.

Uses [cheerio](https://github.com/cheeriojs/cheerio) to parse HTML and [UglifyJS](https://github.com/mishoo/UglifyJS) to uglify JS code.

## Installation

Install package with NPM and add it to your development dependencies:

`npm install --save-dev gulp-uglify-inline`

## Usage

```javascript
var uglifyInline = require('gulp-uglify-inline');

gulp.task('uglify-html', function() {
  gulp.src('./*.html')
    .pipe(uglifyInline())
    .pipe(gulp.dest('dist'))
});
```

## LICENSE

[MIT License](http://en.wikipedia.org/wiki/MIT_License)
