---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
	.version('beta')
	.header('ConsistencyLevel','eventual')
	.filter('startswith(displayName,'a'),')
	.orderby('displayName ')
	.top(1)
	.get();

```