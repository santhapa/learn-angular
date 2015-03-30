## Hello World Example

## Code

```html
<!doctype html>
<html>
<head>
   <script src="js/angular.min.js"></script>
</head>
<body ng-app="myapp">
   <h2>Angular Js <i>Hello World</i></h2>
   
   <div ng-controller="HelloController" >
        <h2>Hello {{ world }}</h2>
   </div>
   <script>
      angular.module("myapp", [])
      .controller("HelloController", function($scope) {
         $scope.world = 'World';
      });
   </script>


</body>
</html>
```

## Include AngularJS
We have included the AngularJS JavaScript file in the HTML page so we can use AngularJS:

```html
<head>
   <script src="js/angular.min.js"></script>
</head>
```
Check the latest version of AngularJS on their official website.

## Point to AngularJS app

Next we tell what part of the HTML contains the AngularJS app. This done by adding the ng-app attribute to the root HTML element of the AngularJS app. You can either add it to html element or body element as shown below:

```html
<body ng-app="myapp">
</body>
```

### View

The view is this part:

```html
<div ng-controller="HelloController" >
   <h2>Hello {{ world }}</h2>
</div>
```
ng-controller tells AngularJS what controller to use with this view. helloTo.title tells AngularJS to write the "model" value named helloTo.title to the HTML at this location.

### Controller

The controller part is:

```js
<script>
   angular.module("myapp", [])
   .controller("HelloController", function($scope) {
      $scope.world = 'World';
   });
</script>
```

This code registers a controller function named HelloController in the angular module named myapp. The controller function is registered in angular via the angular.module(...).controller(...) function call.

The $scope parameter passed to the controller function is the model. The controller function adds a helloTo JavaScript object, and in that object it adds a title field.

**Refer `hello-world.html`**
