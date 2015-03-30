## Hello World Example

## Code

```
<!doctype html>
<html>
   	<head>
      	<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.0-beta.17/angular.min.js"></script>
   	</head>
   	<body ng-app="myapp">
      	<div ng-controller="HelloController" >
         	<h2>Welcome {{helloTo.title}} to the world of Tutorialspoint!</h2>
      	</div>
      	<script>
         	angular.module("myapp", [])
         		.controller("HelloController", function($scope) {
            	$scope.helloTo = {};
            	$scope.helloTo.title = "AngularJS";
         	});
      	</script>
   	</body>
</html>

```

## Include AngularJS
We have included the AngularJS JavaScript file in the HTML page so we can use AngularJS:

```
<head>
   <script src="http://ajax.googleapis.com/ajax/libs/angularjs/1.3.14/angular.min.js"></script>
</head>
```
Check the latest version of AngularJS on their official website.

## Point to AngularJS app

Next we tell what part of the HTML contains the AngularJS app. This done by adding the ng-app attribute to the root HTML element of the AngularJS app. You can either add it to html element or body element as shown below:

```
<body ng-app="myapp">
</body>
```

### View

The view is this part:

```
<div ng-controller="HelloController" >
   <h2>Welcome {{helloTo.title}} to the world of Tutorialspoint!</h2>
</div>
```
ng-controller tells AngularJS what controller to use with this view. helloTo.title tells AngularJS to write the "model" value named helloTo.title to the HTML at this location.

### Controller

The controller part is:

```
<script>
   angular.module("myapp", [])
   .controller("HelloController", function($scope) {
      $scope.helloTo = {};
      $scope.helloTo.title = "AngularJS";
    });
</script>
```

This code registers a controller function named HelloController in the angular module named myapp. The controller function is registered in angular via the angular.module(...).controller(...) function call.

The $scope parameter passed to the controller function is the model. The controller function adds a helloTo JavaScript object, and in that object it adds a title field.