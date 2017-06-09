# Favorite

## Add Product into Favorite

> Sample Request

```shell
curl "https://carikotak.com/api/favorite/10?type=product"
  -X "PUT"
```

#### HTTP REQUEST

- `PUT https://carikotak.com/api/favorite/{id}?type=product`

#### PARAMETERS
Parameter   |   |   Description
--------    | - |   -----------
id  | required  | product ID

#### QUERIES
Query   |   |   Description
----    | - |   -----------
type    | required  | string value 'product' or 'post'. Default 'product'


## Remove Product from Favorite

> Sample Request

```shell
curl "https://carikotak.com/api/favorite/10?type=product"
  -X "DELETE"
```

#### HTTP REQUEST

- `DELETE https://carikotak.com/api/favorite/{id}?type=product`

#### PARAMETERS
Parameter   |   |   Description
--------    | - |   -----------
id  | required  | product ID

#### QUERIES
Query   |   |   Description
----    | - |   -----------
type    | required  | string value 'product' or 'post'. Default 'product'


## Add Post into Favorite

> Sample Request

```shell

curl "https://carikotak.com/api/favorite/20?type=post"
-X "PUT"

```

#### HTTP REQUEST

- `PUT https://carikotak.com/api/favorite/{id}?type=post`

#### PARAMETERS
Parameter   |   |   Description
--------    | - |   -----------
id  | required  | post ID

#### QUERIES
Query   |   |   Description
----    | - |   -----------
type    | required  | string value 'product' or 'post'. Default 'product'


## Remove Product from Favorite

> Sample Request

```shell

curl "https://carikotak.com/api/favorite/20?type=post"
-X "DELETE"

```

#### HTTP REQUEST

- `DELETE https://carikotak.com/api/favorite/{id}?type=post`

#### PARAMETERS
Parameter   |   |   Description
--------    | - |   -----------
id  | required  | post ID

#### QUERIES
Query   |   |   Description
----    | - |   -----------
type    | required  | string value 'product' or 'post'. Default 'product'

