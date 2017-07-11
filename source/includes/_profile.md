# Profile

## Get Profile Info

> Sample Request

```shell
curl "https://carikotak.com/api/me"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/me`

## Get Profile Favorite Posts

> Sample Request

```shell
curl "https://carikotak.com/api/me/favorite-posts"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/me/favorite-posts

## Get Profile Favorite Products

> Sample Request

```shell
curl "https://carikotak.com/api/me/favorite-products"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/me/favorite-products`

## Get Profile Followings

> Sample Request

```shell
curl "https://carikotak.com/api/me/followings"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/me/followings`

## Get Profile Followers

> Sample Request

```shell
curl "https://carikotak.com/api/me/followers"
  -X "GET"
```

#### HTTP REQUEST
- `GET https://carikotak.com/api/me/followers`

## Change Password

> Sample Request

```shell
curl "https://carikotak.com/api/me/change-password"
  -X "PUT"
```

#### HTTP REQUEST
- `PUT https://carikotak.com/api/me/change-password`

#### PARAMETERS

Parameter |  | Description
--------- | ------- | -----------
current_password  | required  | User Current Password
new_password  | required  | User New Password
confirm_password  | required  | Confirm User new password

## Update Profile Info

> Sample Request

```shell
curl "https://carikotak.com/api/me/update-profile"
  -X "PUT"
```

#### HTTP REQUEST
- `PUT https://carikotak.com/api/me/update-profile`

#### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
name  | required  | user name
email | required  | user email (must not have been used by anyone)
description | optional  | user description
city_id | optional  | city id must already exists in database or error (can be null)
province_id | optional  | province id must already exists in database or error (can be null)
