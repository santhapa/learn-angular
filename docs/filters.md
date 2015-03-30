## Filters

Filters are used to modify the data. They can be clubbed in expression or directives using pipe (|) character. 

- **uppercase** converts a text to upper case text.
- **lowercase** converts a text to lower case text.
- **currency** formats text in a currency format.
- **filter** filter the array to a subset of it based on provided criteria.
- **orderby** orders the array based on provided criteria.

```html
	<p>{{ item | uppercase }}</p>
	<p>{{ item | lowercase }}</p>
	<p>{{ price | currency }}</p>
	<li ng-repeat="brand in brands |filter:name">
	<li ng-repeat="brand in brands |orderBy:'name'">
```

**Refer `filters.html`**
[Go here!](../filters.html)
[Back to Index](index.md)
