# Product

## Get All Products

> Sample Request

```shell
curl "https://carikotak.com/product"
  -X "GET"
```

## Get a Specific Product

> Sample Request

```shell
curl "https://carikotak.com/product/{slug}"
  -X "GET"
```

## Store a New Product

> Sample Request

```shell
curl "https://carikotak.com/product/create"
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

### HTTP REQUEST
`POST http://carikotak.com/product/create`

### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
name | required | Product name
price | required | Product price
category_id | required | Product Category
material | optional | Product material
color | optional | Product color
image | optional | Product image
description | required | Product description
type | required | Product type

## Update Existing Product

> Sample Request

```shell
curl "https://carikotak.com/product/{id}"
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

### HTTP REQUEST
`PUT http://carikotak.com/product/{id}`

### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
name | required | Product name
price | required | Product price
category_id | required | Product Category
material | optional | Product material
color | optional | Product color
image | optional | Product image
description | required | Product description
type | required | Product type

## Remove Product

> Sample Request

```shell
curl "https://carikotak.com/product/{id}"
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
