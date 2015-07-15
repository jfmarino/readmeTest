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

Refer to Backbone's [save method](http://backbonejs.org/#Model-save) documentation for more information.
