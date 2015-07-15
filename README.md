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
  limit: 10,
  offset: 0,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MODELNAMEAll.fetch({
  query: {
    FIELDNAME: FIELDVALUE // here the query is passed as an attribute on the single options hash
  },
  limit: 10,
  offset: 0,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});
```

The first object passed represents the field values to match when executing the query. The second object is an options hash, where you can define `success` and `error` callbacks but also a `limit` and `offset` value if you want the query results to be paginated.

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.

#####MODELNAMEExactMatch

Get a Collection with instances that match the query exactly. The difference with the Read action is that it returns a Colleciton, not just a single Model. You may execute this query scope by calling the `query` method or the `fetch` method.

```javascript
var MODELNAMEExactMatch = new SDKNAMESdk.collections.MODELNAMEExactMatch();

// using the query method
MODELNAMEExactMatch.query({
  FIELDNAME: FIELDVALUE
}, {
  limit: 10,
  offset: 0,
  success: function(collection, response, options) {...},
  error: function(collection, response, options) {...}
});

// using the fetch method
MODELNAMEExactMatch.fetch({
  query: {
    FIELDNAME: FIELDVALUE // here the query is passed as an attribute on the single options hash
  },
  limit: 10,
  offset: 0,
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

Refer to [Backbone's Collection fetch method](http://backbonejs.org/#Collection-fetch) documentation for more information.
