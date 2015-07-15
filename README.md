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

Refer to [Backbone's save method](http://backbonejs.org/#Model-save) documentation for more information.

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

Refer to [Backbone's save method](http://backbonejs.org/#Model-save) documentation for more information.

####Read
