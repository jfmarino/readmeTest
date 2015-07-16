<!-- TOC depth:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Developing with Grunt](#developing-with-grunt)
	- [Prerequisites](#prerequisites)
	- [Install NodeJS Modules](#install-nodejs-modules)
	- [Build for Production](#build-for-production)
	- [Development](#development)
	- [Automatic Compilation & Testing](#automatic-compilation-testing)
	- [Running Tests](#running-tests)
- [Using the SDK](#using-the-sdk)
	- [Working with Data](#working-with-data)
		- [Working with](#working-with-j-objectdefinitionname-)
	- [Authentication:  Login & Logout](#authentication-login-logout)
<!-- /TOC -->

#SDKNAMESdk

##Setup

To initialize the SDK you must first provide a base URL for your backend server. Then, all you need to do is call the init method on SDKNAMESdk.

```javascript
SDKNAMESdk.baseUrl = "https://www.foo.com";
SDKNAMESdk.init();
```

If your application is *DirectToSource* then you can skip the base URL setup.

##Using local caching

Local caching can be toggled easily by setting the value of the Application variable `useOfflineCache` **before** initializing the SDK.

```javascript
SDKNAMESdk.useOfflineCache = true;
SDKNAMESdk.init();
```

If you would like to activate it **after** initialization, you can use the method `initOfflineCache` on the SDK.

```javascript
SDKNAMESdk.initOfflineCache();
```

Keep in mind that once local caching has been enabled it cannot be disabled in runtime.

##Models

Available Model objects:

* MODELNAME

###MODELNAME

####Create

This is an example of how you would create a MODELNAME Model.

```javascript
var exampleModel = new SDKNAMESdk.models.MODELNAME();

exampleModel.save({ "ATTRIBUTENAME": TYPEVALUE }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `ATTRIBUTENAME` in the Model to `TYPEVALUE` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "ATTRIBUTENAME": TYPEVALUE }, {
  async: false, // execute this request synchronously
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Update

Updating a MODELNAME Model is very similar to creating one. Updating is done by calling the save method on an already persisted object. 

```javascript
exampleModel.save({ "ATTRIBUTENAME": TYPEVALUE2 });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "ATTRIBUTENAME": TYPEVALUE2 }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "ATTRIBUTENAME": TYPEVALUE2 }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single MODELNAME instance by its primary key.

```javascript
var singleInstance = new SDKNAMESdk.models.MODELNAME({
  id: 1
});

singleInstance.fetch({
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
singleInstance.fetch({
  async: false,
  success: function(model, response, options) {
    // after the model has been fetched from the server...
  },
  error: function(model, response, options) {
    // handle fetch error...
  }
});
```

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

####Delete

In order to delete a single model from the server you can call either the `delete` or `destroy` methods on a Model. Both methods will have the same outcome.

```javascript
// using delete
exampleModel.delete({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

The `success` and `error` callback are optional as with other Backbone CRUD method calls.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
// using delete
exampleModel.delete({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});

// using destroy
exampleModel.destroy({
  async: false,
  success: function(model, response, options) {...},
  error: function(model, response, options) {...}
});
```

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.

####Query Scopes

The available query scopes for MODELNAME objects are:

* MODELNAMEAll
* MODELNAMEExactMatch
* MODELNAMECount
* MODELNAMECountExactMatch

#####MODELNAMEAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MODELNAMEAll = new SDKNAMESdk.collections.MODELNAMEAll();

// using the query method
MODELNAMEAll.query({
  FIELDNAME: FIELDVALUE
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MODELNAMEAll.fetch({
  query: {
    FIELDNAME: FIELDVALUE // here the query is passed as an attribute on the single options hash
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MODELNAMEAll.query({
  FIELDNAME: FIELDVALUE
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.

#####MODELNAMEExactMatch

Get a Collection with instances that match the query exactly. The difference with the Read action is that it returns a Colleciton, not just a single Model. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MODELNAMEExactMatch = new SDKNAMESdk.collections.MODELNAMEExactMatch();

// using the query method
MODELNAMEExactMatch.query({
  FIELDNAME: FIELDVALUE
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MODELNAMEExactMatch.fetch({
  query: {
    FIELDNAME: FIELDVALUE // here the query is passed as an attribute on the single options hash
  },
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MODELNAMEExactMatch.query({
  FIELDNAME: FIELDVALUE
}, {
  async: false,
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.

#####MODELNAMECount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MODELNAMECount = new SDKNAMESdk.collections.MODELNAMECount();

// using the query method
MODELNAMECount.query({
  FIELDNAME: FIELDVALUE
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MODELNAMECount.fetch({
  query: {
    FIELDNAME: FIELDVALUE // here the query is passed as an attribute on the single options hash
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = MODELNAMECount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MODELNAMECount.query({
  FIELDNAME: FIELDVALUE
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = MODELNAMECount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.

#####MODELNAMECountExactMatch

Get the amount of instances that match the given query exactly. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MODELNAMECountExactMatch = new SDKNAMESdk.collections.MODELNAMECountExactMatch();

// using the query method
MODELNAMECountExactMatch.query({
  FIELDNAME: FIELDVALUE
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MODELNAMECountExactMatch.fetch({
  query: {
    FIELDNAME: FIELDVALUE // here the query is passed as an attribute on the single options hash
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = MODELNAMECountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
MODELNAMECountExactMatch.query({
  FIELDNAME: FIELDVALUE
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = MODELNAMECountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.

####Value interpolation

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var MODELNAMEInstance = new SDKNAMESdk.models.MODELNAME();
MODELNAMEInstance.save(
  null, // passing null means we want to save all attributes
  { // options
    interpolationContext: [
      {foo: bar},
      window
    ]
  }
);
```

**Note:** the interpolation context is always an *Array* of *Objects*. Those objects will be collapsed into a single Object which will then act as the context, so [{a: "a", b: "b", c: "c"}, {b: "B", d: "D"}] will end up as {a: "a", b: "B", c: "c", d: "D"}. Note that the Object with the highest index in the Array will overwrite previous ones.

Another way to set the interpolation context is to set it on a MODELNAME instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
MODELNAMEInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of MODELNAME to use the same context, you can set it in the prototype:

```javascript
SDKNAMESdk.models.MODELNAME.prototype.interpolationContext = [{foo: bar}, window];
```
