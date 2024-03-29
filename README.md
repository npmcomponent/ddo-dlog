*This repository is a mirror of the [component](http://component.io) module [ddo/dlog](http://github.com/ddo/dlog). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/ddo-dlog`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
dlog
====

a Simple &amp; Beautiful Logging for Browser

![](https://raw2.github.com/ddo/dlog/master/readme_img/feature.png)

## Features

* Super Lightweight (<2kb)
* Colorful.
* Font size customize.
* Timestamp.
* Log levels: trace, debug, info, warn, error.
* Silent mode. (for production)
* Limit logs by level.

## Installation

### Manual

Download dlog.js [here](https://raw2.github.com/ddo/dlog/0.1.1/dlog.min.js)

    <script src="dlog.min.js"></script>
    
### Bower

    bower install dlog
    
### Component

    component install ddo/dlog

### Init

```js
var log = new dlog();
```

## Levels (in order)

* trace
* debug
* info
* warn
* error
* silent

## Usage

### init

```js
var log = new dlog({
	name: "App Name",
	size: 20, //font size
	level: "info"
});
```

### .log(level, data)

```js
log.log('info', data);
```

```js
log.log('debug', data]);
```

...

### .{level}(data)

```js
log.trace(data);
```

```js
log.warn(data);
```

```js
log.error(data);
```

...

### .setSize()

* Default: 14px
* Set font size

```js
log.setSize(19);
```

### .setName()

* Default: "DLOG"
* Set App name, you may have many apps to log.

```js
log.setName("App Name");
```

### .setLevel()

* Default: "info"
* Set logging level to limit the showing log.
* For example, if logging level is "info" then all the "trace" and "debug" level logs will not be showed.
* Set level to "silent" to stop all log. (good for production)

```js
log.setLevel("silent");
```
## Examples

### log.trace

![](https://raw2.github.com/ddo/dlog/master/readme_img/trace.png)

### log.debug

![](https://raw2.github.com/ddo/dlog/master/readme_img/debug.png)

### log.info

![](https://raw2.github.com/ddo/dlog/master/readme_img/info.png)

### log.warn

![](https://raw2.github.com/ddo/dlog/master/readme_img/warn.png)

### log.error

![](https://raw2.github.com/ddo/dlog/master/readme_img/error.png)

### log.silent

Nothing !!!

### Table

Table will show if data is a array of objects

![](https://raw2.github.com/ddo/dlog/master/readme_img/table.png)

### Todo

* Customize level.
* Color Setting.
* Log format templates.

## License

MIT © [Ddo](http://ddo.me)


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/ddo/dlog/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

