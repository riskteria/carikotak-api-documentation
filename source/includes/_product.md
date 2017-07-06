# Product

## Product List

> Sample Request

```shell
curl "https://carikotak.com/api/product"
  -X "GET"

curl "https://carikotak.com/api/product?user=10"
-X "GET"

curl "https://carikotak.com/api/product?page=10&per_page=10"
-X "GET"

```

#### HTTP REQUEST
- `GET https://carikotak.com/api/product`
- `GET https://carikotak.com/api/product?user={userId}`
- `GET https://carikotak.com/api/product?page={int}&per_page={int}`

#### QUERIES
Query   | Type  | Description
--------| ----- | -----------
user    | optional  | Get product list from user
page    | optional  | Pagination page, default 0
per_page | optional | Number of results per page, default 10


## Read Product

> Sample Request

```shell
curl "https://carikotak.com/api/product/show-me-your-product"
  -X "GET"
```

#### HTTP REQUEST
`GET https://carikotak.com/api/product/{slug}`


## Store Product

> Sample Request

```shell
curl "https://carikotak.com/api/product/"
  -X "POST"
```

> Success Response

```shell
{
    "status": "ok",
    "message": "product has been added",
    "product": "{object}"
}
```

> Fail Response

```shell
{
    'status': 'error',
    'message': 'product cannot be added'
}
```

#### HTTP REQUEST
`POST https://carikotak.com/api/product`

#### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
name | required | Product name
price | required | Product price
category_id | required | Product Category
description | required | Product description
type | required | 'jual' or 'cari'
condition | required | 'new' or 'second'
material | optional | Product material
color | optional | Product color
image | optional | Product image (array)
width | optional | Product Width
length | optional | Product Length
weight | optional | Product Weight
height | optinoal | product Height

## Update Product

> Sample Request

```shell
curl "https://carikotak.com/product/1"
  -X "PUT"
```

> Success Response

```shell
{
    "status": "ok",
    "message": "product has been updated",
    "product": "{object}"
}
```

> Fail Response

```shell
{
    'status': 'error',
    'message': 'product cannot be updated'
}
```

#### HTTP REQUEST
`PUT http://carikotak.com/api/product/{id}`

#### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
name | required | Product name
price | required | Product price
category_id | required | Product Category
description | required | Product description
material | optional | Product material
color | optional | Product color
image | optional | Product image
type | required | Product type

## Remove Product

> Sample Request

```shell
curl "https://carikotak.com/product/1"
  -X "DELETE"
```

> Success Response

```shell
{
    'status': 'ok',
    'message': 'product deleted successfully'
}
```

> Fail Response

```shell
{
    'status': 'error',
    'message': 'product cannot be deleted'
}
``` 

#### HTTP REQUEST
`DELETE https://carikotak.com/api/product/{productId}`
