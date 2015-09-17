# RelationshipsSdk

## Description

This should serve as a guide for the Angular SDK for `Relationships`

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
      - [Running Tests](#running-tests)
- [Testing](#testing)

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
	* **lib** - Dependencies
	* **model** - Model module
	* **models** - *Generated Models*
	* **utility** - Utility module
* **test** - SDK unit tests for generic modules and classes as well as generated Models

## <a name="adding-the-sdk-to-your-application"></a> Adding the SDK to your Application

In order to include this SDK within your Application simply take the file `ap_sdk.js`, found in the SDK folder at the root level. This file contains the entire SDK code in one file **without** the dependencies like Angular. Take that file and copy it anywhere you want within you Application folder structure and just include it in your `index.html` using a <scripṭ/\> tag.

### <a name="dependencies"></a> Dependencies

All the SDK dependencies can be found in the path *SDK_ROOT/sdk/lib/*, where SDK_ROOT is the folder where this SDK is. You must add this dependencies for the SDK to work properly, however, note that you can download this dependencies yourself if you wish, you don't **have** to use the ones in the lib folder specifically, they are included there as a convenience.

## <a name="setup-and-initialize-the-sdk"></a> Setup and Initialize the SDK

To setup the SDK within your application, first you need to declare

```javascript
angular.module("myApp", ["RelationshipsSdk"]);
```

That will give you access to your Model services from Controllers, Factories, Services and so on. To use the SDK you must first provide a base URL for your backend server. You can do this by calling `$relationshipsSdkConfig.baseUrl.set()`

```javascript
angular.module("myApp")
	.controller("MyController", ["$relationshipsSdkConfig", function($relationshipsSdkConfig) {

		$relationshipsSdkConfig.baseUrl.set("https://www.foo.com");

	}]);
```

## <a name="local-caching"></a> Local Caching

To have local caching on your SDK you just need to enable it. Bear in mind that local caching only caches GET requests.

Local caching is enabled and/or disabled ***globally***.

```javascript
angular.module("myApp")
	.controller("MyController", ["$relationshipsSdkConfig", function($relationshipsSdkConfig) {

		// Enable local caching
		$relationshipsSdkConfig.offlineCache.enable();
		// You can also disable it at any time
		$relationshipsSdkConfig.offlineCache.disable();

	}]);
```

## <a name="authentication"></a> Authentication

Before you can authenticate with the SDK in your application  you must create an Auth Object in the Anypresence Designer and a user in your application's back end.

```javascript
angular.module("myApp")
  .controller("MyController", ["$relationshipsSdkAuthentication", function($relationshipsSdkAuthentication) {

    // To login
    $relationshipsSdkAuthentication.login({
      username: "johndoe",
      password: "doe123"
    });

    $relationshipsSdkAuthentication.isAuthenticated();
    // true

    // To logout
    $relationshipsSdkAuthentication.logout();

    $relationshipsSdkAuthentication.isAuthenticated();
    // false

	}]);
```

## <a name="models"></a> Models

Available Model objects:

* Cat
* Dog
* Person

### <a name="cat"></a>`Cat`

To use this model you have to inject `$cat`.

#### <a name="create-cat"></a>Create

To create instances of `Cat` do:

```javascript
// The instance does not get saved to the server when created
var instance = $cat.create({ name: "John" });
instance.lastName = "Doe";
instance.age = 28;
// To save the instance do
instance.$save().then(function() {
	// The instance got saved
});
```

#### <a name="read-cat"></a>Read

To read a specific instance by id you can do:

```javascript
$cat.get({ id: "1" }).then(function(response) {
	// The instance with id = "1" got fetched
	// instance data is in response.data
	console.log(response.data);
});
```

#### <a name="update-cat"></a>Update

To update an instance you can call `instance.$save()` at any time. Updating will be triggered if the instance has an `id` field that is not `undefined`.

```javascript
// To update the instance pass an object containing the attributes you want to update to the $save method
instance.$save({
  age: 29
}).then(function() {
	// The instance got updated
});
```

#### <a name="delete-cat"></a>Delete

To delete an instance:

```javascript
$cat.delete({ id: "1" }).then(function() {
	// The instance with id = "1" got deleted from the server
});
```

#### <a name="direct-to-source-cat"></a>Direct to Source

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

Aside from passing an interpolation context, CRUD methods and query scopes work exactly the same way as before.

This is how you would specify the interpolation context for the different ***CRUD*** methods and query scopes:

##### Create

```javascript
// The object passed to $save() will be used as the interpolation context
instance.$save({
  foo: "bar"
});
```

##### Read

```javascript
// The object passed to get() as argument will be the interpolation context
$cat.get({ foo: "bar" });
```

##### Update

```javascript
// The object passed to $save() will be used as the interpolation context
instance.$save({
  foo: "bar"
});
```

##### Delete

```javascript
// The object passed to delete() as argument will be the interpolation context
$cat.delete({ foo: "bar" });
```

##### Query Scopes

Query scopes on direct to source Models work almost exactly the same as on regular Models. The difference is that instead of passing an object like:

```javascript
{
  query: {
    id: 1
  },
  limit: 10,
  offset: 0
}
```

You would instead pass an interpolation context to the scope

```javascript
// The object passed to all() will be used as the interpolation context
$scope.myScope = $cat.all({
  foo: "bar"
});
```

#### <a name="query-scopes-cat"></a>Query Scopes

The available query scopes for `Cat` are:

* all
* exact_match
* count
* count_exact_match

##### `CatAll`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $cat.CatAll();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $cat.CatAll({
	query: { // In query go the parameters for the scope
		name: "John",
		age: 40
	},
	// Pagination options
	limit: 15, // Max amount of results
	offset: 0,	// The index from which to start reading the amount of elements
}, function(collection) { // Success callback
	// Use the collection data returned
}, function(err) { // Error callback
	// There was an error while fetching the data
});
```


##### `CatExactMatch`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $cat.CatExactMatch();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $cat.CatExactMatch({
	query: { // In query go the parameters for the scope
		name: "John",
		age: 40
	},
	// Pagination options
	limit: 15, // Max amount of results
	offset: 0,	// The index from which to start reading the amount of elements
}, function(collection) { // Success callback
	// Use the collection data returned
}, function(err) { // Error callback
	// There was an error while fetching the data
});
```


##### `CatCount`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $cat.CatCount();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```

##### `CatCountExactMatch`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $cat.CatCountExactMatch();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```


#### <a name="relationships-cat"></a>Relationships

To access relationships within a Model there is an object within __all__ Models called `$related` that holds the defined relationships. Relationships act like query scopes, you can pass success and error callbacks to any of them and they always return an empty Array that will be filled when the request returns from the server.


##### Belongs To


###### `Person`

```javascript
$cat.$related.person(function(result) {
	// result will be an Array with the related models
	console.log("Success!!");
}, function() {
	console.log("Error :(");
});
```




### <a name="dog"></a>`Dog`

To use this model you have to inject `$dog`.

#### <a name="create-dog"></a>Create

To create instances of `Dog` do:

```javascript
// The instance does not get saved to the server when created
var instance = $dog.create({ name: "John" });
instance.lastName = "Doe";
instance.age = 28;
// To save the instance do
instance.$save().then(function() {
	// The instance got saved
});
```

#### <a name="read-dog"></a>Read

To read a specific instance by id you can do:

```javascript
$dog.get({ id: "1" }).then(function(response) {
	// The instance with id = "1" got fetched
	// instance data is in response.data
	console.log(response.data);
});
```

#### <a name="update-dog"></a>Update

To update an instance you can call `instance.$save()` at any time. Updating will be triggered if the instance has an `id` field that is not `undefined`.

```javascript
// To update the instance pass an object containing the attributes you want to update to the $save method
instance.$save({
  age: 29
}).then(function() {
	// The instance got updated
});
```

#### <a name="delete-dog"></a>Delete

To delete an instance:

```javascript
$dog.delete({ id: "1" }).then(function() {
	// The instance with id = "1" got deleted from the server
});
```

#### <a name="direct-to-source-dog"></a>Direct to Source

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

Aside from passing an interpolation context, CRUD methods and query scopes work exactly the same way as before.

This is how you would specify the interpolation context for the different ***CRUD*** methods and query scopes:

##### Create

```javascript
// The object passed to $save() will be used as the interpolation context
instance.$save({
  foo: "bar"
});
```

##### Read

```javascript
// The object passed to get() as argument will be the interpolation context
$dog.get({ foo: "bar" });
```

##### Update

```javascript
// The object passed to $save() will be used as the interpolation context
instance.$save({
  foo: "bar"
});
```

##### Delete

```javascript
// The object passed to delete() as argument will be the interpolation context
$dog.delete({ foo: "bar" });
```

##### Query Scopes

Query scopes on direct to source Models work almost exactly the same as on regular Models. The difference is that instead of passing an object like:

```javascript
{
  query: {
    id: 1
  },
  limit: 10,
  offset: 0
}
```

You would instead pass an interpolation context to the scope

```javascript
// The object passed to all() will be used as the interpolation context
$scope.myScope = $dog.all({
  foo: "bar"
});
```

#### <a name="query-scopes-dog"></a>Query Scopes

The available query scopes for `Dog` are:

* all
* exact_match
* count
* count_exact_match

##### `DogAll`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $dog.DogAll();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $dog.DogAll({
	query: { // In query go the parameters for the scope
		name: "John",
		age: 40
	},
	// Pagination options
	limit: 15, // Max amount of results
	offset: 0,	// The index from which to start reading the amount of elements
}, function(collection) { // Success callback
	// Use the collection data returned
}, function(err) { // Error callback
	// There was an error while fetching the data
});
```


##### `DogExactMatch`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $dog.DogExactMatch();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $dog.DogExactMatch({
	query: { // In query go the parameters for the scope
		name: "John",
		age: 40
	},
	// Pagination options
	limit: 15, // Max amount of results
	offset: 0,	// The index from which to start reading the amount of elements
}, function(collection) { // Success callback
	// Use the collection data returned
}, function(err) { // Error callback
	// There was an error while fetching the data
});
```


##### `DogCount`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $dog.DogCount();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```

##### `DogCountExactMatch`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $dog.DogCountExactMatch();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```


#### <a name="relationships-dog"></a>Relationships

To access relationships within a Model there is an object within __all__ Models called `$related` that holds the defined relationships. Relationships act like query scopes, you can pass success and error callbacks to any of them and they always return an empty Array that will be filled when the request returns from the server.


##### Belongs To


###### `Person`

```javascript
$dog.$related.person(function(result) {
	// result will be an Array with the related models
	console.log("Success!!");
}, function() {
	console.log("Error :(");
});
```




### <a name="person"></a>`Person`

To use this model you have to inject `$person`.

#### <a name="create-person"></a>Create

To create instances of `Person` do:

```javascript
// The instance does not get saved to the server when created
var instance = $person.create({ name: "John" });
instance.lastName = "Doe";
instance.age = 28;
// To save the instance do
instance.$save().then(function() {
	// The instance got saved
});
```

#### <a name="read-person"></a>Read

To read a specific instance by id you can do:

```javascript
$person.get({ id: "1" }).then(function(response) {
	// The instance with id = "1" got fetched
	// instance data is in response.data
	console.log(response.data);
});
```

#### <a name="update-person"></a>Update

To update an instance you can call `instance.$save()` at any time. Updating will be triggered if the instance has an `id` field that is not `undefined`.

```javascript
// To update the instance pass an object containing the attributes you want to update to the $save method
instance.$save({
  age: 29
}).then(function() {
	// The instance got updated
});
```

#### <a name="delete-person"></a>Delete

To delete an instance:

```javascript
$person.delete({ id: "1" }).then(function() {
	// The instance with id = "1" got deleted from the server
});
```

#### <a name="direct-to-source-person"></a>Direct to Source

On DirectToSource Models you can specify certain values of the request being made to use string interpolation, but you also need a way of specifying what the context is going to be during that operation.

Aside from passing an interpolation context, CRUD methods and query scopes work exactly the same way as before.

This is how you would specify the interpolation context for the different ***CRUD*** methods and query scopes:

##### Create

```javascript
// The object passed to $save() will be used as the interpolation context
instance.$save({
  foo: "bar"
});
```

##### Read

```javascript
// The object passed to get() as argument will be the interpolation context
$person.get({ foo: "bar" });
```

##### Update

```javascript
// The object passed to $save() will be used as the interpolation context
instance.$save({
  foo: "bar"
});
```

##### Delete

```javascript
// The object passed to delete() as argument will be the interpolation context
$person.delete({ foo: "bar" });
```

##### Query Scopes

Query scopes on direct to source Models work almost exactly the same as on regular Models. The difference is that instead of passing an object like:

```javascript
{
  query: {
    id: 1
  },
  limit: 10,
  offset: 0
}
```

You would instead pass an interpolation context to the scope

```javascript
// The object passed to all() will be used as the interpolation context
$scope.myScope = $person.all({
  foo: "bar"
});
```

#### <a name="query-scopes-person"></a>Query Scopes

The available query scopes for `Person` are:

* all
* exact_match
* count
* count_exact_match

##### `PersonAll`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $person.PersonAll();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $person.PersonAll({
	query: { // In query go the parameters for the scope
		name: "John",
		age: 40
	},
	// Pagination options
	limit: 15, // Max amount of results
	offset: 0,	// The index from which to start reading the amount of elements
}, function(collection) { // Success callback
	// Use the collection data returned
}, function(err) { // Error callback
	// There was an error while fetching the data
});
```


##### `PersonExactMatch`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $person.PersonExactMatch();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $person.PersonExactMatch({
	query: { // In query go the parameters for the scope
		name: "John",
		age: 40
	},
	// Pagination options
	limit: 15, // Max amount of results
	offset: 0,	// The index from which to start reading the amount of elements
}, function(collection) { // Success callback
	// Use the collection data returned
}, function(err) { // Error callback
	// There was an error while fetching the data
});
```


##### `PersonCount`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $person.PersonCount();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```

##### `PersonCountExactMatch`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $person.PersonCountExactMatch();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```


#### <a name="relationships-person"></a>Relationships

To access relationships within a Model there is an object within __all__ Models called `$related` that holds the defined relationships. Relationships act like query scopes, you can pass success and error callbacks to any of them and they always return an empty Array that will be filled when the request returns from the server.



##### Has One


###### Cat

```javascript
$person.$related.cat(function(result) {
	// result will be an Array with the related models
	console.log("Success!!");
}, function() {
	console.log("Error :(");
});
```


##### Has Many


###### Dog

```javascript
$person.$related.dogs(function(result) {
	// result will be an Array with the related models
	console.log("Success!!");
}, function() {
	console.log("Error :(");
});
```



## <a name="development"></a> Development

### Developing with Grunt

Grunt is a NodeJS-based task runner.  It helps automate common tasks, such as
asset compilation, minification, and testing.  Grunt tasks are included for this
SDK in `Gruntfile.js`.

Follow the directions below to get up and running with Grunt.

#### Prerequisites

- [NodeJS](http://nodejs.org)

#### Install NodeJS Modules

From the root directory of the SDK (where `Gruntfile.js` is
located), install NodeJS modules:

`npm install`

#### Adding code to the SDK

In order to add additional files to the final SDK build all that is required is to include the file within the building process.
The build process is actually just concatenation of all the modules and files that comprise the SDK, so to add more you can modify Gruntfile.js found in the root of the SDK folder.

```javascript
concat: {
  javascript: {
    src: [
      /**
      * Static
      */
      'sdk/utility/utility.module.js',
      ...
      ...
      /**
      * Generated
      */
      'sdk/adapters/adapters.module.js',
      ...
      ...
      /**
      * Custom added files
      */
      'path/to/my/code.js',
      ...
    ],
    dest: 'ap_sdk.js'
  }
},
```

#### Build for Production

To compile assets and create a full production build, run the
build task:

`grunt build`

#### Development

During development, a full minified SDK build is unnecessary.  To
compile assets without minifying:

`grunt compile`

#### Automatic Compilation

Since it's cumbersome to manually compile assets after every change during
development, the SDK's `Gruntfile.js` includes a `watch` task.  The
task monitors changes to the SDK's `coffee` and `sass` assets,
automatically compiling (but not minifying) them.  Run the following command
before making changes:

`grunt watch`

## <a name="testing"></a> Testing

The SDK comes with a complete test suite.  Execute tests from grunt:

`grunt test`

SDK tests are also executed by the `watch` task.  If changing the SDK
significantly, some or all tests may fail.  You may disable auto-testing by
editing the `watch` task in `Gruntfile.js`.

The test suite can also be run directly in a browser.  Open `test/index.html` and click
"Run Tests".
