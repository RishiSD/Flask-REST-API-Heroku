# Stores REST Api

This is built with Flask, Flask-RESTful, Flask-JWT and Flask-SQLAlchemy

Deployed on Heroku https://stores-rest-api-rishi.herokuapp.com/.

# Documentation

## Resources

### Item
#### Attributes
`name`_`(string)`_: Name of the item.<br>
`price`_`(float)`_: Price of the item in USD.<br>
`store_id`_`(int)`_: Unique ID for a store.

#### Endpoints
__`GET`__`/item/<string:name>`: Get an item by passing item name.<br>
__`POST`__`/item/<string:name>`: Add a new item using item name.<br>
__`PUT`__`/item/<string:name>`: Add or update an item using item name.<br>
__`DELETE`__`/item/<string:name>`: Delete an item using item name.<br>
__`GET`__`/items`: Get a list of all the items.

### Store
#### Attributes
`name`_`(string)`_: Name of the store.<br>
`items`_`(array)`_: List of items in the store.

#### Endpoints
__`GET`__`/store/<string:name>`: Get store by passing store name.<br>
__`POST`__`/store/<string:name>`: Add a new store using store name.<br>
__`DELETE`__`/store/<string:name>`: Delete a store using store name.<br>
__`GET`__`/stores`: Get a list of all the stores.

### User
#### Attributes
`username`_`(string)`_: Name of the API user.<br>
`password`_`(string)`_: Password of the API user.

#### Endpoints
__`POST`__`/register`: Add or Register a user to get JWT token for add, update or delete activities.
