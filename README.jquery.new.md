# RelationshipsSdk

## Description

This should serve as a guide for the JQuery SDK for `Relationships`

## Table of Contents


- [Project Structure](#project-structure)
- [Adding the SDK to your Application](#adding-the-sdk-to-your-application)
    - [Dependencies](#dependencies)
- [Setup and Initialize the SDK](#setup-and-initialize-the-sdk)
- [Local Caching](#local-caching)
- [Authentication](#authentication)
- [Models](#models)
		
      	- [Cat](#cat)
		- [Create](#create-cat)
      		- [Read](#read-cat)
		- [Update](#update-cat)
		- [Delete](#delete-cat)
      		- [Direct to Source](#direct-to-source-cat)
		- [Query Scopes](#query-scopes-cat)
			
		- [Relationships](#relationships-cat)
			
		
	- [Dog](#dog)
		- [Create](#create-dog)
      		- [Read](#read-dog)
		- [Update](#update-dog)
		- [Delete](#delete-dog)
      		- [Direct to Source](#direct-to-source-dog)
		- [Query Scopes](#query-scopes-dog)
			
		- [Relationships](#relationships-dog)
			
		
	- [Person](#person)
		- [Create](#create-person)
      		- [Read](#read-person)
		- [Update](#update-person)
		- [Delete](#delete-person)
      		- [Direct to Source](#direct-to-source-person)
		- [Query Scopes](#query-scopes-person)
		- [Relationships](#relationships-person)
			
- [Development](#development)
    - [Developing with Grunt](#developing-with-grunt)
      - [Prerequisites](#prerequisites)
      - [Install NodeJS Modules](#install-nodejs-modules)
      - [Adding code to the SDK](#adding-code-to-the-sdk)
      - [Build for Production](#build-for-production)
      - [Development](#development)
      - [Automatic Compilation & Testing](#automatic-compilation-testing)
- [Testing](#testing)
- [Troubleshooting](#troubleshooting)
- [Miscellaneous](#miscellaneous)

## <a name="project-structure"></a> Project Structure

General description of the files and folders you will find within this SDK project folder.

* ap_sdk.js - The main SDK file, this contains all the code for this SDK except for third-party dependencies
* **custom** - Convenience folder where you can keep any additional code to add to this SDK
* **docs** - This folder contains all the documentation generated, you will find a web-based guide you can open on your browser
* Gruntfile.js - Grunt configuration and tasks, if you want to add code to this SDK you can use Grunt for development
* LICENSE.txt - The SDK license
* **node_modules** - NPM dependencies for development and testing
* package.json - The library definition manifest containing description, version and dependencies of this SDK
* README.md - This file
* **sdk** - Here you will find all the SDK code
	* **adapter** - AP.adapter module
	* **adapters** - *Generated adapters*
	* **ap** - Anypresence namespace definition
	* **application** - Application class definition
	* **auth** - Authentication module
	* **collection** - Collection module
	* **collections** - *Generated Collections*
	* **lib** - Dependencies
	* **model** - Model module
	* **models** - *Generated Models*
	* **relationship** - Relationship module
	* **utility** - Utility module
* **test** - SDK unit tests for generic modules and classes as well as generated Models and Collections

## <a name="adding-the-sdk-to-your-application"></a> Adding the SDK to your Application

In order to include this SDK within your Application simply take the file `ap_sdk.js`, found in the SDK folder at the root level. This file contains the entire SDK code in one file **without** the dependencies like JQuery. Take that file and copy it anywhere you want within you Application folder structure and just include it in your `index.html` using a <scripṭ/\> tag.

### <a name="dependencies"></a> Dependencies

All the SDK dependencies can be found in the path *SDK_ROOT/sdk/lib/*, where SDK_ROOT is the folder where this SDK is. You must add this dependencies for the SDK to work properly, however, note that you can download this dependencies yourself if you wish, **you don't have to use** the ones in the lib folder specifically, they are included there as a convenience.

## <a name="setup-and-initialize-the-sdk"></a> Setup and Initialize the SDK

To initialize the SDK you must first provide a base URL for your backend server. Then, all you need to do is call the init method on RelationshipsSdk.

```javascript
AP.baseUrl = "https://www.foo.com";
RelationshipsSdk.init();
```

If your application is *DirectToSource* then you can skip the base URL setup.

## <a name="local-caching"></a> Local Caching

Local caching can be toggled easily by setting the value of the Application variable `useOfflineCache` **before** initializing the SDK.

```javascript
RelationshipsSdk.useOfflineCache = true;
RelationshipsSdk.init();
```

If you would like to activate it **after** initialization, you can use the method `initOfflineCache` on the SDK.

```javascript
RelationshipsSdk.initOfflineCache();
```

Keep in mind that once local caching has been enabled it cannot be disabled in runtime.

## <a name="authentication"></a> Authentication

Before you can authenticate with the SDK in your application  you must create an Auth Object in the Anypresence Designer and a user in your application's back end.

```javascript
// login
AP.auth.Authentication.login({
  username: 'test',
  password: 'password'
});

// logout
AP.auth.Authentication.logout();
```

## <a name="models"></a> Models

Available Model objects:

* Cat
* Dog
* Person


### `Cat`

#### Create

To create instances of `Cat` do:

```javascript
var exampleModel = new RelationshipsSdk.models.Cat();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

#### Read

To read a specific instance by id you can do:

```javascript
var singleInstance = new RelationshipsSdk.models.Cat({
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

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

#### Update

Updating a Cat Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

#### Delete

To delete an instance:

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

#### <a name="direct-to-source-cat"></a>Direct to Source

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var CatInstance = new RelationshipsSdk.models.Cat();
CatInstance.save(
  null, // passing null means we want to save all attributes
  { // options
    interpolationContext: [
      {foo: bar},
      window
    ]
  }
);
```

**Note:** the interpolation context is always an *Array* of *Objects*. Those objects will be collapsed into a single Object which will then act as the context, so `[{a: "a", b: "b", c: "c"}, {b: "B", d: "D"}]` will end up as `{a: "a", b: "B", c: "c", d: "D"}`. Note that the Object with the highest index in the Array will overwrite previous ones.

Another way to set the interpolation context is to set it on a Cat instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
CatInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of Cat to use the same context, you can set it in the prototype:

```javascript
RelationshipsSdk.models.Cat.prototype.interpolationContext = [{foo: bar}, window];
```

#### <a name="query-scopes-cat"></a>Query Scopes

The available query scopes for `Cat` are:

* all
* exact_match
* count
* count_exact_match

##### `CatAll`


```javascript
var CatAll = new RelationshipsSdk.collections.CatAll();

CatAll.fetch({
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

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


##### `CatExactMatch`


```javascript
var CatExactMatch = new RelationshipsSdk.collections.CatExactMatch();

CatExactMatch.fetch({
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

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


##### `CatCount`


```javascript
var CatCount = new RelationshipsSdk.collections.CatCount();

CatCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the value
var value = CatCount.valueOf();
```

##### `CatCountExactMatch`


```javascript
var CatCountExactMatch = new RelationshipsSdk.collections.CatCountExactMatch();

CatCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the value
var value = CatCountExactMatch.valueOf();
```



#### <a name="relationships-cat"></a>Relationships

##### Belongs To


###### `person`

```javascript
var modelInstance = new RelationshipsSdk.models.Cat();
modelInstance.getRelationship("person").fetch(function(owner, parent) {
  // parent is the object modelInstance belongs to...
});
```





### `Dog`

#### Create

To create instances of `Dog` do:

```javascript
var exampleModel = new RelationshipsSdk.models.Dog();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

#### Read

To read a specific instance by id you can do:

```javascript
var singleInstance = new RelationshipsSdk.models.Dog({
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

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

#### Update

Updating a Dog Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

#### Delete

To delete an instance:

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

#### <a name="direct-to-source-dog"></a>Direct to Source

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var DogInstance = new RelationshipsSdk.models.Dog();
DogInstance.save(
  null, // passing null means we want to save all attributes
  { // options
    interpolationContext: [
      {foo: bar},
      window
    ]
  }
);
```

**Note:** the interpolation context is always an *Array* of *Objects*. Those objects will be collapsed into a single Object which will then act as the context, so `[{a: "a", b: "b", c: "c"}, {b: "B", d: "D"}]` will end up as `{a: "a", b: "B", c: "c", d: "D"}`. Note that the Object with the highest index in the Array will overwrite previous ones.

Another way to set the interpolation context is to set it on a Dog instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
DogInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of Dog to use the same context, you can set it in the prototype:

```javascript
RelationshipsSdk.models.Dog.prototype.interpolationContext = [{foo: bar}, window];
```

#### <a name="query-scopes-dog"></a>Query Scopes

The available query scopes for `Dog` are:

* all
* exact_match
* count
* count_exact_match

##### `DogAll`


```javascript
var DogAll = new RelationshipsSdk.collections.DogAll();

DogAll.fetch({
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

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


##### `DogExactMatch`


```javascript
var DogExactMatch = new RelationshipsSdk.collections.DogExactMatch();

DogExactMatch.fetch({
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

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


##### `DogCount`


```javascript
var DogCount = new RelationshipsSdk.collections.DogCount();

DogCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the value
var value = DogCount.valueOf();
```

##### `DogCountExactMatch`


```javascript
var DogCountExactMatch = new RelationshipsSdk.collections.DogCountExactMatch();

DogCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the value
var value = DogCountExactMatch.valueOf();
```



#### <a name="relationships-dog"></a>Relationships

##### Belongs To


###### `person`

```javascript
var modelInstance = new RelationshipsSdk.models.Dog();
modelInstance.getRelationship("person").fetch(function(owner, parent) {
  // parent is the object modelInstance belongs to...
});
```





### `Person`

#### Create

To create instances of `Person` do:

```javascript
var exampleModel = new RelationshipsSdk.models.Person();

exampleModel.save({ "id": "foo" }, {
  success: function(model, response, options) {
    // handle save success...
  },
  error: function(model, response, options) {
    // handle error...
  }
});
```

Refer to [Backbone's Model save method](http://backbonejs.org/#Model-save) documentation for more information.

#### Read

To read a specific instance by id you can do:

```javascript
var singleInstance = new RelationshipsSdk.models.Person({
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

Refer to [Backbone's Model fetch method](http://backbonejs.org/#Model-fetch) documentation for more information.

#### Update

Updating a Person Model is very similar to creating one. Updating is done by calling the save method on an already persisted object.

```javascript
exampleModel.save({ "id": "foo" });
```

Updating the Model this way will cause a `PUT` request to be triggered, if you would like to send a `PATCH` request instead, then you should call like so:

```javascript
exampleModel.save({ "id": "foo" }, {patch: true});
```

Just like in Model creation, even if you are not updating all Model attributes, a complete representation is sent to the server.

#### Delete

To delete an instance:

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

#### <a name="direct-to-source-person"></a>Direct to Source

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

The interpolation context can be set in more than one way. If you would like to specify a context to be used for a specific call you would do:

```javascript
var PersonInstance = new RelationshipsSdk.models.Person();
PersonInstance.save(
  null, // passing null means we want to save all attributes
  { // options
    interpolationContext: [
      {foo: bar},
      window
    ]
  }
);
```

**Note:** the interpolation context is always an *Array* of *Objects*. Those objects will be collapsed into a single Object which will then act as the context, so `[{a: "a", b: "b", c: "c"}, {b: "B", d: "D"}]` will end up as `{a: "a", b: "B", c: "c", d: "D"}`. Note that the Object with the highest index in the Array will overwrite previous ones.

Another way to set the interpolation context is to set it on a Person instance, if you would like that instance to always use the same context you can just set it like this:

```javascript
PersonInstance.interpolationContext = [{foo: bar}, window];
```

This way you don't have to set it on every call.

The next step is, if you would like **all** instances of Person to use the same context, you can set it in the prototype:

```javascript
RelationshipsSdk.models.Person.prototype.interpolationContext = [{foo: bar}, window];
```

#### <a name="query-scopes-person"></a>Query Scopes

The available query scopes for `Person` are:

* all
* exact_match
* count
* count_exact_match

##### `PersonAll`


```javascript
var PersonAll = new RelationshipsSdk.collections.PersonAll();

PersonAll.fetch({
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

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


##### `PersonExactMatch`


```javascript
var PersonExactMatch = new RelationshipsSdk.collections.PersonExactMatch();

PersonExactMatch.fetch({
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

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.


##### `PersonCount`


```javascript
var PersonCount = new RelationshipsSdk.collections.PersonCount();

PersonCount.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the value
var value = PersonCount.valueOf();
```

##### `PersonCountExactMatch`


```javascript
var PersonCountExactMatch = new RelationshipsSdk.collections.PersonCountExactMatch();

PersonCountExactMatch.fetch({
  query: { // here the query is passed as an attribute on the single options hash
    
  },
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// to access the value
var value = PersonCountExactMatch.valueOf();
```



#### <a name="relationships-person"></a>Relationships


##### Has One


###### cat

```javascript
var modelInstance = new RelationshipsSdk.models.Person();
modelInstance.getRelationship("cat").fetch(function(owner, relatedObject) {
  // relatedObject belongs to modelInstance
});
```

##### Has Many

###### dogs

```javascript
var modelInstance = new RelationshipsSdk.models.Person();
modelInstance.getRelationship("dogs").fetch(function(owner, relatedObjects) {
  // relatedObjects is a collection
});
```



## <a name="development"></a> Development

This sections shows the dependencies and steps to develop or modify this SDK.

### Developing with Grunt

Grunt is a NodeJS-based task runner.  It helps automate common tasks, such as
asset compilation, minification, and testing.  Grunt tasks are included for this
SDK in `Gruntfile.js`.

Follow directions below to get up and running with Grunt.

#### Prerequisites

- [NodeJS](http://nodejs.org)

#### Install NodeJS Modules

From the root directory of the SDK (where `Gruntfile.js` is
located), install NodeJS modules:

    npm install

#### Adding code to the SDK

In order to add additional files to the final SDK build all that is required is to include the file within the building process.
The build process is actually just concatenation of all the modules and files that comprise the SDK, so to add more you can modify `Gruntfile.js` found in the root of the SDK folder.

```
concat: {
  javascript: {
    src: [
      // A lot of files that make the SDK are listes here
      'sdk/ap/**.js',
      ...
      // You can add your files anywhere you want within the list they don't need to be at the bottom
      // However, note that if your code depends on any of the default SDK code you will need to add it after all the other files
      // or at least after the stuff you depend on.
      'path/to/my/code.js',
      ...
    ],
    dest: 'ap_sdk.js'
  }
},
```

After you add your files, just build the SDK with the steps below and your code will be added to `ap_sdk.js`

#### Build for Production

To compile assets and create a full production build, run the
build task:

    grunt build

#### Automatic Compilation & Testing

Since it's cumbersome to manually compile assets after every change during
development, the SDK's `Gruntfile.js` includes a `watch` task.  The
task monitors changes to the SDK's `coffee` and `sass` assets,
automatically compiling (but not minifying) them.  Run the following command
before making changes:

    grunt watch

## <a name="testing"></a> Testing

The SDK comes with a complete test suite.  Execute tests from grunt:

`grunt test`

SDK tests are also executed by the `watch` task.  If changing the SDK
significantly, some or all tests may fail.  You may disable auto-testing by
editing the `watch` task in `Gruntfile.js`.

The test suite can also be run directly in a browser.  Open `test/index.html` and click
"Run Tests".

## <a name="troubleshooting"></a> Troubleshooting

***[Section describing how to troubleshoot issues encountered while developing with the SDK]***
