# Post

## Post List

> Sample Request

```shell

curl "https://carikotak.com/api/post"
  -X "GET"

curl "https://carikotak.com/api/post?user=23"
  -X "GET"

curl "https://carikotak.com/api/post?page=1&per_page=10"
  -X "GET"

curl "https://carikotak.com/api/post?keyword=hello&page=1&per_page=10"
  -X "GET"

```

#### HTTP REQUEST
- `GET https://carikotak.com/api/post`
- `GET https://carikotak.com/api/post?user={user_id}`
- `GET https://carikotak.com/api/post?page={page_number}&per_page={number_per_page}`
- `GET https://carikotak.com/api/post?keyword={text}`

#### QUERIES
Query   | Type  | Description
--------| ----- | -----------
user    | optional  | Get post list from user
page    | optional  | Pagination page, default 0
per_page | optional | Number of results per page, default 10
keyword | optional  | Keyword used to search posts

## Read Post

> Sample Request

```shell
curl "https://carikotak.com/api/post/this-is-a-sample-post"
  -X "GET"
```

#### HTTP REQUEST
`GET https://carikotak.com/api/post/{slug}`

## Create Post

> Sample Request

```shell
curl "https://carikotak.com/api/post"
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

#### HTTP REQUEST
`POST http://carikotak.com/api/post/`

#### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
category_id | required | Post Category
title | required | Post title
body | required | Post body
image | optional | Product image

## Update Post

> Sample Request

```shell
curl "https://carikotak.com/api/post/{postId}"
  -X "PUT"
```

> Success Response

```shell
{
    "status": "ok",
    "message": "post has been updated",
    "product": "{object}"
}
```

> Fail Response

```shell
{
    'status': 'error',
    'message': 'post cannot be updated'
}
```

#### HTTP REQUEST
`PUT http://carikotak.com/post/1`

#### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
category_id | required | Post Category
title | required | Post title
body | required | Post body
image | optional | Product image

## Remove Post

> Sample Request

```shell
curl "https://carikotak.com/api/post/{postId}"
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

#### HTTP REQUEST
`DELETE https://carikotak.com/api/post/{postId}`