# Comment

## Get Product Comment List

> Sample Request

```shell
curl "https://carikotak.com/api/product/23/comment"
  -X "GET"
```

#### HTTP REQUEST

- `GET https://carikotak.com/api/product/{product_id}/comment`

## Get Post Comment List

> Sample Request

```shell
curl "https://carikotak.com/api/post/23/comment"
  -X "GET"
```

#### HTTP REQUEST

- `GET https://carikotak.com/api/post/{post_id}/comment`

## Comment on a Product

> Sample Request

```shell
curl "https://carikotak.com/api/comment"
  -X "POST"
```

#### HTTP REQUEST

- `POST https://carikotak.com/api/comment`

#### PARAMETERS
Parameter   |   |   Description
--------    | - |   -----------
target_id   | required  | target product ID or post ID
target_type | required  | 'product'
comment     | required  | comment text

## Comment on a Post

> Sample Request

```shell
curl "https://carikotak.com/api/comment"
  -X "POST"
```

#### HTTP REQUEST

- `POST https://carikotak.com/api/comment`

#### PARAMETERS
Parameter   |   |   Description
--------    | - |   -----------
target_id   | required  | target product ID or post ID
target_type | required  | 'post'
comment     | required  | comment text

## Delete Comment

> Sample Request

```shell
curl "https://carikotak.com/api/comment/30"
  -X "DELETE"
```

#### HTTP REQUEST

- `DELETE https://carikotak.com/api/comment/{id_comment}`