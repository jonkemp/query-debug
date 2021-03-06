# jquery-debug [![Build Status](https://travis-ci.org/jonkemp/jquery-debug.svg?branch=master)](https://travis-ci.org/jonkemp/jquery-debug)

> A plugin that makes jQuery throw an error, rather than fail silently, when a selector returns no results.

## What is this useful for ?

Save tons of time and frustration debugging jQuery!

## Additional information
- Compatible with jQuery 1.x-2.x. Not compatible with 3.0 yet.
- Not for use in production (obviously).

## Install

Install with [npm](https://npmjs.org/package/jquery-debug)

```bash
npm install --save jquery-debug
```

Check out this article for more information on [how to use jQuery plugins with npm](http://blog.npmjs.org/post/112064849860/using-jquery-plugins-with-npm).

## Usage

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>demo</title>
  <script src="https://code.jquery.com/jquery-2.2.4.js"></script>
</head>
<body>

<div>DIV</div>

<script>
var element = $('p').debug();
</script>

</body>
</html>
```

Here's the error message you would see in the browser console.

```
jquery-debug: The jQuery selector 'p' was not found in the context of '#document'.
```

For a live example, check out the [CodePen](http://codepen.io/jonkemp/pen/PzZdLQ?editors=1010).

## Contributing

See the [CONTRIBUTING Guidelines](https://github.com/jonkemp/inline-css/blob/master/CONTRIBUTING.md)

## License

MIT © [Jonathan Kemp](http://jonkemp.com)
