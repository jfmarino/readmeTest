# ThemableSdk

## Description

This should serve as a guide for the Angular SDK for `Themable`

## Table of Contents


- [Project Structure](#project-structure)
- [Adding the SDK to your Application](#adding-the-sdk-to-your-application)
    - [Dependencies](#dependencies)
- [Setup and Initialize the SDK](#setup-and-initialize-the-sdk)
- [Local Caching](#local-caching)
- [Ajax Settings](#ajax-settings)
- [Authentication](#authentication)
- [File Uploads](#file-uploads)
- [Models](#models)

	- [Employee](#employee)
		- [Create](#create-employee)
		- [Read](#read-employee)
    	- [Update](#update-employee)
		- [Delete](#delete-employee)
    	- [Query Scopes](#query-scopes-employee)
		
	
- [Development](#development)
    - [Developing with Grunt](#developing-with-grunt)
      - [Prerequisites](#prerequisites)
      - [Install NodeJS Modules](#install-nodejs-modules)
      - [Adding code to the SDK](#adding-code-to-the-sdk)
      - [Build for Production](#build-for-production)
      - [Manual Compilation](#manual-compilation)
      - [Automatic Compilation](#automatic-compilation)
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
angular.module("myApp", ["ThemableSdk"]);
```

That will give you access to your Model services from Controllers, Factories, Services and so on. To use the SDK you must first provide a base URL for your backend server. You can do this by calling `$themableSdkConfig.baseUrl.set()`

```javascript
angular.module("myApp")
	.controller("MyController", ["$themableSdkConfig", function($themableSdkConfig) {

		$themableSdkConfig.baseUrl.set("https://www.foo.com");

	}]);
```

## <a name="local-caching"></a> Local Caching

To have local caching on your SDK you just need to enable it. Bear in mind that local caching only caches GET requests.

Local caching is enabled and/or disabled ***globally***.

```javascript
angular.module("myApp")
	.controller("MyController", ["$themableSdkConfig", function($themableSdkConfig) {

		// Enable local caching
		$themableSdkConfig.offlineCache.enable();
		// You can also disable it at any time
		$themableSdkConfig.offlineCache.disable();

	}]);
```

## <a name="ajax-settings"></a> Ajax Settings

You can also modify the global ajax settings for your SDK. Here is an example

```javascript
angular.module("myApp")
  .controller("MyController", ["$themableSdkConfig", function($themableSdkConfig) {
    $themableSdkConfig.ajaxSettings({
      headers: { "Foo": "Bar" },
      data: { "hello": "world" },
      withCredentials: true
    });
  }]);
```

The available settings are

* headers -> object
* params -> object
* data -> object
* withCredentials -> boolean
* requestTransformations -> Array of functions
* responseTransformations -> Array of functions

## <a name="authentication"></a> Authentication

Before you can authenticate with the SDK in your application  you must create an Auth Object in the Anypresence Designer and a user in your application's back end.

```javascript
angular.module("myApp")
  .controller("MyController", ["$themableSdkAuthentication", function($themableSdkAuthentication) {

    // To login
    $themableSdkAuthentication.login({
      username: "johndoe",
      password: "doe123"
    });

    $themableSdkAuthentication.isAuthenticated();
    // true

    // To logout
    $themableSdkAuthentication.logout();

    $themableSdkAuthentication.isAuthenticated();
    // false

	}]);
```

## <a name="file-uploads"></a> File Uploads

Models in the SDK may have fields which are files. Uploading files is already baked into the Model class, so just set that field to a file and use the `.$save()` method in the model. If you would like to remove a file, just set that same field to `null` and save it. You may need to use a directive to pull the files from an input type="file". Once a file has been uploaded, the contents of that field will be replaced for a URI string to locate the file itself.

Here's an example of how you can save a Model containing file fields. First we need to obtain the file from an input with type file

HTML
```html
<!-- Modeling a candidate for a job listing  -->
<!-- the first name of the candidate -->
<input type="text" ng-model="name">
<!-- the last name of the candidate -->
<input type="text" ng-model="lastname">
<!-- the candidate's resume -->
<input type="file" file-upload>
```

JS
```javascript
angular.module("myApp")
.directive('fileUpload', function () {
    return {
        scope: true,  //create a new scope
        link: function (scope, el, attrs) {
            el.bind('change', function (event) {
                var files = event.target.files;
                if(files && files.length) {
                  // emit the last file selected with the input
                  scope.$emit("fileSelected", { file: files[i] });
                }
            });
        }
    };
})
.controller("TestController", ["$scope", "$candidate", function($scope, $candidate) {

  $scope.name = undefined;
  $scope.lastname = undefined;
  $scope.resume = undefined;

  //listen for the file selected event
  $scope.$on("fileSelected", function (event, args) {
      $scope.$apply(function () {
          // set the resume as the emitted file
          $scope.resume = args.file;
      });
  });

  $scope.create = function() {
    var attr = { name: $scope.name, lastname: $scope.lastname, resume: $scope.resume };
    var newCandidate = $candidate.create(attr);
    newCandidate
      .$save()
      .then(function() {
        // model got saved correctly
        // now if we inspect the resume field we will see that a url string came back directing to the resource
        console.log(newCandidate.resume);
      })
      .catch(function(err) {
        // there was an error
      });
  };

}]);
```

Now when we get an instance `$candidate.get(...)`, all fields that are of type file will return as a URL to that file. For now the angular sdk does not support pulling the file data unfortunately.

## <a name="models"></a> Models

Available Model objects:

* Employee

### <a name="employee"></a>`Employee`

To use this model you have to inject `$employee`.


#### <a name="create-employee"></a>Create

To create instances of `Employee` do:

```javascript
// The instance does not get saved to the server when created
var instance = $employee.create({ name: "John" });
instance.lastName = "Doe";
instance.age = 28;
// To save the instance do
instance.$save().then(function() {
	// The instance got saved
});
```

#### <a name="read-employee"></a>Read

To read a specific instance by id you can do:

```javascript
$employee.get({ id: "1" }).then(function(response) {
	// The instance with id = "1" got fetched
	// instance data is in response.data
	console.log(response.data);
});
```

#### <a name="update-employee"></a>Update

To update an instance you can call `instance.$save()` at any time. Updating will be triggered if the instance has an `id` field that is not `undefined`.

```javascript
// To update the instance pass an object containing the attributes you want to update to the $save method
instance.$save({
  age: 29
}).then(function() {
	// The instance got updated
});
```

#### <a name="delete-employee"></a>Delete

To delete an instance:

```javascript
$employee.delete({ id: "1" }).then(function() {
	// The instance with id = "1" got deleted from the server
});
```


#### <a name="query-scopes-employee"></a>Query Scopes


The available query scopes for `Employee` are:

* all
* exact_match
* count
* count_exact_match

##### `all`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $employee.all();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $employee.all({
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


##### `exact_match`


To fetch the values of a query scope you can just call the query scope from the model. Object scopes like this one return an empty Array that will get filled when the data comes back from the backend server.

```javascript
$scope.myScope = $employee.exact_match();
```

If the scope supports parameters to filter the results, then you can call them like so:

```javascript
$scope.myScope = $employee.exact_match({
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


##### `count`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $employee.count();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```

##### `count_exact_match`


To fetch the values of a query scope you can just call the query scope from the model. Aggregate scopes like this one return an Object with a single attribute. This attribute is always called `value` and it gets filled with the result of the query once the request comes back from the backend server.

```javascript
$scope.myScope = $employee.count_exact_match();
console.log($scope.myScope.value); // Would print a value like "3000" or undefined if the request hasn't returned yet
```





## <a name="development"></a> Development

### <a name="developing-with-grunt"></a> Developing with Grunt

Grunt is a NodeJS-based task runner.  It helps automate common tasks, such as
asset compilation, minification, and testing.  Grunt tasks are included for this
SDK in `Gruntfile.js`.

Follow the directions below to get up and running with Grunt.

#### <a name="prerequisites"></a> Prerequisites

- [NodeJS](http://nodejs.org)

#### <a name="install-nodejs-modules"></a> Install NodeJS Modules

From the root directory of the SDK (where `Gruntfile.js` is
located), install NodeJS modules:

`npm install`

#### <a name="adding-code-to-the-sdk"></a> Adding code to the SDK

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

#### <a name="build-for-production"></a> Build for Production

To compile assets and create a full production build, run the
build task:

`grunt build`

#### <a name="manual-compilation"></a> Manual Compilation

During development, a full minified SDK build is unnecessary.  To
compile assets without minifying:

`grunt compile`

#### <a name="automatic-compilation"></a> Automatic Compilation

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
