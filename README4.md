#AnimeNewsNetworkEncyclopediaSdk

## Table of Contents

<!-- TOC depth:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [AnimeNewsNetworkEncyclopediaSdk](#animenewsnetworkencyclopediasdk)
	- [Table of Contents](#table-of-contents)
	- [Developing with Grunt](#developing-with-grunt)
		- [Prerequisites](#prerequisites)
		- [Install NodeJS Modules](#install-nodejs-modules)
		- [Build for Production](#build-for-production)
		- [Development](#development)
		- [Automatic Compilation & Testing](#automatic-compilation-testing)
		- [Running Tests](#running-tests)
	- [Setup](#setup)
	- [Authentication:  Login & Logout](#authentication-login-logout)
	- [Using local caching](#using-local-caching)
	- [Models](#models)
  
    
		- [AnimeDetail](#anime-detail)
			- [Create](#create)
			- [Update](#update)
			- [Read](#read)
			- [Delete](#delete)
			- [Query Scopes](#query-scopes)
	    
	      
				- [AnimeDetailAll](#animedetailall)
	    
	      
				- [AnimeDetailExactMatch](#animedetailexactmatch)
	    
	      
				- [AnimeDetailCount](#animedetailcount)
	    
	      
				- [AnimeDetailCountExactMatch](#animedetailcountexactmatch)
	    
	      
				- [AnimeDetailAllEpisodes](#animedetailallepisodes)
	    
	    
	    
	    
			- [Value interpolation](#value-interpolation)
	    
    
<!-- /TOC -->

## Developing with Grunt

Grunt is a NodeJS-based task runner.  It helps automate common tasks, such as
asset compilation, minification, and testing.  Grunt tasks are included for this
SDK in `Gruntfile.js`.

Follow directions below to get up and running with Grunt.

### Prerequisites

- [NodeJS](http://nodejs.org)

### Install NodeJS Modules

From the root directory of the SDK (where `Gruntfile.js` is
located), install NodeJS modules:

    npm install

### Build for Production

To compile assets and create a full production build, run the
build task:

    grunt build

### Development

During development, a full minified SDK build is unnecessary.  To
compile assets without minifying:

    grunt compile

### Automatic Compilation & Testing

Since it's cumbersome to manually compile assets after every change during
development, the SDK's `Gruntfile.js` includes a `watch` task.  The
task monitors changes to the SDK's `coffee` and `sass` assets,
automatically compiling (but not minifying) them.  Run the following command
before making changes:

    grunt watch

SDK tests are also executed by the `watch` task.  If changing the SDK
significantly, some or all tests may fail.  You may disable auto-testing by
editing the `watch` task in `Gruntfile.js`.

### Running Tests

The SDK comes with a complete test suite.  Execute tests from grunt:

    grunt test

Or execute tests directly in a browser.  Open `test/index.html` and click
"Run Tests".

##Setup

To initialize the SDK you must first provide a base URL for your backend server. Then, all you need to do is call the init method on AnimeNewsNetworkEncyclopediaSdk.

```javascript
AnimeNewsNetworkEncyclopediaSdk.baseUrl = "https://www.foo.com";
AnimeNewsNetworkEncyclopediaSdk.init();
```

If your application is *DirectToSource* then you can skip the base URL setup.

## Authentication:  Login & Logout
```javascript
AP.auth.Authentication.login({
  username: 'test',
  password: 'password'
});

AP.auth.Authentication.logout();
```

##Using local caching

Local caching can be toggled easily by setting the value of the Application variable `useOfflineCache` **before** initializing the SDK.

```javascript
AnimeNewsNetworkEncyclopediaSdk.useOfflineCache = true;
AnimeNewsNetworkEncyclopediaSdk.init();
```

If you would like to activate it **after** initialization, you can use the method `initOfflineCache` on the SDK.

```javascript
AnimeNewsNetworkEncyclopediaSdk.initOfflineCache();
```

Keep in mind that once local caching has been enabled it cannot be disabled in runtime.

##Models

Available Model objects:

* AnimeDetail

###AnimeDetail

####Create

This is an example of how you would create a AnimeDetail Model.

```javascript
var exampleModel = new AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Here we are setting the attribute `id` in the Model to `"foo"` and then saving it. A complete representation of the Model is always sent to the server, regardless of which attributes you set in the save call.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {
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

Updating a AnimeDetail Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
exampleModel.save({ "id": "foo" }, {async: false});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read

Read operations allow you to get a single AnimeDetail instance by its primary key.

```javascript
var singleInstance = new AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail({
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

The available query scopes for AnimeDetail objects are:

* AnimeDetailAll
* AnimeDetailExactMatch
* AnimeDetailCount
* AnimeDetailCountExactMatch
* AnimeDetailAllEpisodes

#####AnimeDetailAll

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AnimeDetailAll = new AnimeNewsNetworkEncyclopediaSdk.collections.AnimeDetailAll();

// using the query method
AnimeDetailAll.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AnimeDetailAll.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
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
AnimeDetailAll.query({
  
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


  
  
   
    
   
  

####Value interpolation

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var AnimeDetailInstance = new AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail();
AnimeDetailInstance.save(
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

Another way to set the interpolation context is to set it on a AnimeDetail instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
AnimeDetailInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of AnimeDetail to use the same context, you can set it in the prototype:

```javascript
AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail.prototype.interpolationContext = [{foo: bar}, window];
```
#####AnimeDetailExactMatch

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AnimeDetailExactMatch = new AnimeNewsNetworkEncyclopediaSdk.collections.AnimeDetailExactMatch();

// using the query method
AnimeDetailExactMatch.query({
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AnimeDetailExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
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
AnimeDetailExactMatch.query({
  
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


  
  
   
    
   
  

####Value interpolation

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var AnimeDetailInstance = new AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail();
AnimeDetailInstance.save(
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

Another way to set the interpolation context is to set it on a AnimeDetail instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
AnimeDetailInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of AnimeDetail to use the same context, you can set it in the prototype:

```javascript
AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail.prototype.interpolationContext = [{foo: bar}, window];
```
#####AnimeDetailCount

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AnimeDetailCount = new AnimeNewsNetworkEncyclopediaSdk.collections.AnimeDetailCount();

// using the query method
AnimeDetailCount.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AnimeDetailCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = AnimeDetailCount.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
AnimeDetailCount.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = AnimeDetailCount.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.

  
  
   
    
   
  

####Value interpolation

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var AnimeDetailInstance = new AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail();
AnimeDetailInstance.save(
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

Another way to set the interpolation context is to set it on a AnimeDetail instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
AnimeDetailInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of AnimeDetail to use the same context, you can set it in the prototype:

```javascript
AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail.prototype.interpolationContext = [{foo: bar}, window];
```
#####AnimeDetailCountExactMatch

Get the amount of instances that satisfy the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AnimeDetailCountExactMatch = new AnimeNewsNetworkEncyclopediaSdk.collections.AnimeDetailCountExactMatch();

// using the query method
AnimeDetailCountExactMatch.query({
  
}, {
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AnimeDetailCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the amount
var amount = AnimeDetailCountExactMatch.valueOf();
```

######Async

This action is asynchronous by default, if you would like to execute it synchronously you can do:

```javascript
AnimeDetailCountExactMatch.query({
  
}, {
  async: false,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

var amount = AnimeDetailCountExactMatch.valueOf();
```

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.

  
  
   
    
   
  

####Value interpolation

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var AnimeDetailInstance = new AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail();
AnimeDetailInstance.save(
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

Another way to set the interpolation context is to set it on a AnimeDetail instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
AnimeDetailInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of AnimeDetail to use the same context, you can set it in the prototype:

```javascript
AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail.prototype.interpolationContext = [{foo: bar}, window];
```
#####AnimeDetailAllEpisodes

Get all results that match the given query. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var AnimeDetailAllEpisodes = new AnimeNewsNetworkEncyclopediaSdk.collections.AnimeDetailAllEpisodes();

// using the query method
AnimeDetailAllEpisodes.query({
  
  "anime": "foo",
  
}, {
  data: {
    limit: 10,
    offset: 0
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
AnimeDetailAllEpisodes.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
    "anime": "foo",
    
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
AnimeDetailAllEpisodes.query({
  
  "anime": "foo",
  
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


  
  
   
    
   
  

####Value interpolation

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var AnimeDetailInstance = new AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail();
AnimeDetailInstance.save(
  null, // passing null means we want to save all attributes
  { // options
    interpolationContext: [
      {foo: bar},
      window
    ]
  }
);
```

**Note:** the interpolation context is always an *Array* of *Objects*. Those objects will be collapsed into a single Object which will then act as the context so `[{a: "a", b: "b", c: "c"}, {b: "B", d: "D"}]` will end up as `{a: "a", b: "B", c: "c", d: "D"}`. Note that the Object with the highest index in the Array will overwrite previous ones.

Another way to set the interpolation context is to set it on a AnimeDetail instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
AnimeDetailInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of AnimeDetail to use the same context, you can set it in the prototype:

```javascript
AnimeNewsNetworkEncyclopediaSdk.models.AnimeDetail.prototype.interpolationContext = [{foo: bar}, window];
```
