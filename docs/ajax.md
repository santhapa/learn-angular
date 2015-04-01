## Making Ajax call 

AngularJS provides $http control which works as a service to read data from the server. Server makes a database call to get the desired records. AngularJS needs data in JSON format. Once the data is ready, $http can be used to get the data from server in the following manner,

```js
	<script type="text/javascript">
		angular.module("myapp", [])
		.controller("apiController", function($scope, $http) {
			var url="json/posts.json";
			$http.get(url).success( function(response) {
				$scope.posts = response.posts;
			});
		});		
	</script>

```

**Refer `../ajax.html`**

[Back to Index](index.md)
