#RelationshipsSdk

## Table of Contents

<!-- TOC depth:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [RelationshipsSdk](#relationshipssdk)
	- [Table of Contents](#table-of-contents)
	- [Project Structure](#project-structure)
	- [Adding the SDK to your Application](#adding-the-sdk-to-your-application)
		- [Dependencies](#dependencies)
	- [Setup](#setup)
	- [Using local caching](#using-local-caching)
	- [Models](#models)
	
		
		- [Cat](#cat)
			- [Create](#create)
			- [Update](#update)
			- [Read](#read)
			- [Delete](#delete)
			- [Query Scopes](#query-scopes)
			
			- [Relationships](#relationships)
			
	
		
		- [Dog](#dog)
			- [Create](#create-1)
			- [Update](#update-1)
			- [Read](#read-1)
			- [Delete](#delete-1)
			- [Query Scopes](#query-scopes-1)
			
			- [Relationships](#relationships-1)
			
	
		
		- [Person](#person)
			- [Create](#create-2)
			- [Update](#update-2)
			- [Read](#read-2)
			- [Delete](#delete-2)
			- [Query Scopes](#query-scopes-2)
			
			- [Relationships](#relationships-2)
			
	
	- [Developing with Grunt](#developing-with-grunt)
		- [Prerequisites](#prerequisites)
		- [Install NodeJS Modules](#install-nodejs-modules)
		- [Build for Production](#build-for-production)
		- [Development](#development)
		- [Automatic Compilation & Testing](#automatic-compilation-testing)
		- [Running Tests](#running-tests)
<!-- /TOC -->

##Project Structure

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

##Adding the SDK to your Application

In order to include this SDK within your Application simply take the file `ap_sdk.js`, found in the SDK folder at the root level. This file contains the entire SDK code in one file **without** the dependencies like JQuery. Take that file and copy it anywhere you want within you Application folder structure and just include it in your `index.html` using a <scripṭ/\> tag.

###Dependencies

All the SDK dependencies can be found in the path *SDK_ROOT/sdk/lib/*, where SDK_ROOT is the folder where this SDK is. You must add this dependencies for the SDK to work properly, however, note that you can download this dependencies yourself if you wish, you don't **have** to use the ones in the lib folder specifically, they are included there as a convenience.

##Setup

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

##Using local caching

To enable local caching for your SDK you just need to enable it. Bare in mind that local caching only caches GET requests.

```javascript
angular.module("myApp")
	.controller("MyController", ["$relationshipsSdkConfig", function($relationshipsSdkConfig) {

		// Enable local caching
		$relationshipsSdkConfig.offlineCache.enable();
		// You can also disable it at any time
		$relationshipsSdkConfig.offlineCache.disable();

	}]);
```

##Models

Available Model objects:

* Cat
* Dog
* Person

###Cat

To use this model you have to inject `$cat`.

####Create

To create instances of Cat do:

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

####Update

To update an instance you can call `instance.$save()` at any time.

####Read

To read a specific instance by id you can do:

```javascript
$cat.get({ id: "1" }).then(function(response) {
	// The instance with id = "1" got fetched
	// instance data is in response.data
	console.log(response.data);
});
```

####Delete

To delete an instance:

```javascript
$cat.delete({ id: "1" }).then(function() {
	// The instance with id = "1" got deleted from the server
});
```

####Query Scopes

The available query scopes for Cat are:

* all
* exact_match
* count
* count_exact_match

#####all

To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $cat.all();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $cat.all({
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

#####exact_match

To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $cat.exact_match();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $cat.exact_match({
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

#####count

To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute.
This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $cat.count();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```
#####count_exact_match

To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute.
This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $cat.count_exact_match();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```

####Relationships

To access relationships within a Model there is an object within __all__ Models called `$related` that holds the defined relationships. Relationships act like query scopes, you can pass success and error callbacks to any of them and they always return an empty Array that will be filled when the request returns from the server.

##### Belongs To

###### Person

```javascript
$cat.$related.person(function(result) {
	// result will be an Array with the related models
	console.log("Success!!");
}, function() {
	console.log("Error :(");
});
```




###Dog

To use this model you have to inject `$dog`.

####Create

To create instances of Dog do:

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

####Update

To update an instance you can call `instance.$save()` at any time.

####Read

To read a specific instance by id you can do:

```javascript
$dog.get({ id: "1" }).then(function(response) {
	// The instance with id = "1" got fetched
	// instance data is in response.data
	console.log(response.data);
});
```

####Delete

To delete an instance:

```javascript
$dog.delete({ id: "1" }).then(function() {
	// The instance with id = "1" got deleted from the server
});
```

####Query Scopes

The available query scopes for Dog are:

* all
* exact_match
* count
* count_exact_match

#####all

To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $dog.all();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $dog.all({
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

#####exact_match

To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $dog.exact_match();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $dog.exact_match({
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

#####count

To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute.
This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $dog.count();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```
#####count_exact_match

To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute.
This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $dog.count_exact_match();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```

####Relationships

To access relationships within a Model there is an object within __all__ Models called `$related` that holds the defined relationships. Relationships act like query scopes, you can pass success and error callbacks to any of them and they always return an empty Array that will be filled when the request returns from the server.

##### Belongs To

###### Person

```javascript
$dog.$related.person(function(result) {
	// result will be an Array with the related models
	console.log("Success!!");
}, function() {
	console.log("Error :(");
});
```




###Person

To use this model you have to inject `$person`.

####Create

To create instances of Person do:

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

####Update

To update an instance you can call `instance.$save()` at any time.

####Read

To read a specific instance by id you can do:

```javascript
$person.get({ id: "1" }).then(function(response) {
	// The instance with id = "1" got fetched
	// instance data is in response.data
	console.log(response.data);
});
```

####Delete

To delete an instance:

```javascript
$person.delete({ id: "1" }).then(function() {
	// The instance with id = "1" got deleted from the server
});
```

####Query Scopes

The available query scopes for Person are:

* all
* exact_match
* count
* count_exact_match

#####all

To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $person.all();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $person.all({
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

#####exact_match

To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $person.exact_match();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $person.exact_match({
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

#####count

To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute.
This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $person.count();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```
#####count_exact_match

To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute.
This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $person.count_exact_match();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```

####Relationships

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
