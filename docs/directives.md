## Angular Js Directives

AngularJS directives are used to extend HTML. They are special attributes starting with ng-prefix. 
**ng-app** - starts an AngularJS Application.
**ng-init** - initializes application data.
**ng-model** - defines the model that is variable to be used in AngularJS.
**ng-bind** - binds the angular ng-model data to Html element.
**ng-repeat** - repeats HTML elements for each item in a collection (basically for array iteration).

### ng-app directive
The ng-app directive starts an AngularJS Application. It defines the root element. It automatically initializes or bootstraps the application when the web page containing AngularJS Application is loaded. It is also used to load various AngularJS modules in AngularJS Application.
```html
<div ng-app="">
	...
</div>
```

### ng-init directive
The ng-init directive initializes an AngularJS Application data. It is used to assign values to the variables.
```html
<div ng-app="" ng-init="names=['Ram', 'Hari', 'Rita']">
	...
</div>
```

### ng-model directive
The ng-model directive defines the model/variable to be used in AngularJS Application.
```html
<div ng-app="">
	...
	<p>Enter your Name: <input type="text" ng-model="name"></p>
</div>
```

### ng-repeat directive
ng-repeat directive repeats HTML elements for each item in a collection.
```html
<div ng-app="">
	...
 	<p>List of Countries with locale:</p>
 	<ol>
 		<li ng-repeat="name in names">
 			{{ name }}
 		</li>
 	</ol>
</div>
```

### ng-bind directive
The ng-bind directive binds the angular variable to html element.
```html
<span ng-bind="name"></span>
<!--similar to {{ name }}  -->
```

[Back to Index](index.md)