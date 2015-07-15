#SDKNAMESdk

##Setup

To initialize the SDK you must first provide a base URL for your backend server. Then, all you need to do is call the init method on SDKNAMESdk.

```javascript
SDKNAMESdk.baseUrl = "https://www.foo.com";
SDKNAMESdk.init();
```

If your application is *DirectToSource* then you can skip the base URL setup.

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

Refer to [Backbone's Model destroy method](http://backbonejs.org/#Model-destroy) documentation for more information.
