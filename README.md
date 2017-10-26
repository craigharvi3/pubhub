# PubHub


## Get Started

In the root of the folder, run the following commands:

### Install dependencies
```
yarn install
```

### Build JS and SASS
```
yarn bundle
```

**Alternatively you can watch assets by:**
```
yarn watch
```

### Start server
```
yarn start
```

**Visit** [http://localhost:8080](http://localhost:8080)

### Linting

```
yarn lint
```

### Tests

```
yarn test
```


## Directory Structure
* `app` - This is where the main application lives (client and server codebase)
    * `client` - The front end code including sass, javascript and images.
    * `server` - The back end code including routes, controllers, models and data stubs.
* `test` - This is where all unit tests live (just front end tests for now).
* `public` - Contains the static index.html and where build files including css, javascript and images are compiled to.


## API Requirements

The following endpoints will be required in order to deliver my magical vision:

* `/api/v1/bars [GET]` - Get bars with optional `s` query param allowing searching.
* `/api/v1/bars/:bar_id [GET]` - Get bar with id `bar_id`.
* `/api/v1/bars/:bar_id/products [GET]` - Get products for `bar_id`.
* `/api/v1/orders [POST]` - Create a new order.
* `/api/v1/orders/:order_id [GET]` - Get order with id `order_id`.
* `/api/v2/orders/:order_id [PUT]` - Update order with id `order_id`.
* `/api/v2/orders/:order_id/products/:product_id [POST]` - Add product to order with `order_id` and `product_id`.
* `/api/v2/orders/:order_id/products/:product_id [DELETE]` - Remove product from order with `order_id` and `product_id`.