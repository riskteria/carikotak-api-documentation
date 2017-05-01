# Post

## Get All Posts

> Sample Request

```shell
curl "https://carikotak.com/post"
  -X "GET"
```

## Get a Specific Post

> Sample Request

```shell
curl "https://carikotak.com/product/{slug}"
  -X "GET"
```

## Store a new Post

> Sample Request

```shell
curl "https://carikotak.com/post/{id}"
  -X "PUT"
```

> Success Response

```shell
{
    "status": "ok",
    "message": "post has been added",
    "product": "{object}"
}
```

> Fail Response

```shell
{
    'status': 'error',
    'message': 'post cannot be added'
}
```

### HTTP REQUEST
PUT http://carikotak.com/post/{id}`

### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
category_id | required | Post Category
title | required | Post title
body | required | Post body
image | optional | Product image

## Update Existing Post

> Sample Request

```shell
curl "https://carikotak.com/post/create"
  -X "POST"
```

> Success Response

```shell
{
    "status": "ok",
    "message": "post has been added",
    "product": "{object}"
}
```

> Fail Response

```shell
{
    'status': 'error',
    'message': 'post cannot be added'
}
```

### HTTP REQUEST
`POST http://carikotak.com/post/create`

### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
category_id | required | Post Category
title | required | Post title
body | required | Post body
image | optional | Product image

## Remove Product

> Sample Request

```shell
curl "https://carikotak.com/post/{id}"
  -X "DELETE"
```

> Success Response

```shell
{
    'status': 'ok',
    'message': 'post deleted successfully'
}
```

> Fail Response

```shell
{
    'status': 'error',
    'message': 'post cannot be deleted'
}
```