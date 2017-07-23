# User

## Get List of User

> Sample Request

```shell
curl "https://carikotak.com/api/user?keyword=hello"
  -X "GET"

curl "https://carikotak.com/api/user?page=1&per_page=10"
  -X "GET"

curl "https://carikotak.com/api/user?keyword=hello&page=1&per_page=10"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/user`
- `GET https://carikotak.com/api/user?page={int}&per_page={int}`
- `GET https://carikotak.com/api/user?keyword={text}`

## Get User Info

> Sample Request

```shell
curl "https://carikotak.com/api/user/historiareiss"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/user/{username}`

## Get User Followers

> Sample Request

```shell
curl "https://carikotak.com/api/user/historiareiss/follower"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/user/{username}/follower`

## Get User Followings

> Sample Request

```shell
curl "https://carikotak.com/api/user/historiareiss/following"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/user/{username}/following`

## Get User Product Comments

> Sample Request

```shell
curl "https://carikotak.com/api/user/historiareiss/comment-product"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/user/{username}/comment-product`

## Get User Post Comments

> Sample Request

```shell
curl "https://carikotak.com/api/user/historiareiss/comment-post"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/user/{username}/comment-post`