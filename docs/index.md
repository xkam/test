# test

Angular 2 - ES5 example

```js

	var Component = require('@angular/core').Component;

	function Hello(){
		this.msg = 'Hello Angular';
	}

	Hello.annotations = [new Component({
		selector: '#app',
		template: '{{msg}}'
	})];

	// --- module ---

	var NgModule = require('@angular/core').NgModule,
		BrowserModule = require('@angular/platform-browser').BrowserModule,
		platformBrowserDynamic = require('@angular/platform-browser-dynamic').platformBrowserDynamic;

	function App (){}

	App.annotations = [new NgModule({
		imports: [BrowserModule],
		declarations: [Hello],
		bootstrap: [Hello]
	})];

	platformBrowserDynamic().bootstrapModule(App);

```

[Open in browser](test.html)
