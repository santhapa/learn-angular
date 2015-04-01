## Embedding Html Pages

Generally, html does not allow for embedding other html pages in it. For that purpose we need to use **Ajax** or other server side includes like **PHP, JSP, etc**.

Through angular js, we can easily include html pages within html page, using **`ng-include`**

```html
<div ng-app="testApp" ng-controller="studentController" >
	<div ng-include="'info.html'"></div>
	<div ng-include="'score.html'"></div>
</div>
```

**Refer [includes](../include-eg/index.html)**

[Back to Index](index.md)

