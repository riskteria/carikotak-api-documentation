# Authentication

Carikotak use API `token` to allow access for required authentication’s resources.

## Register New User

> Sample Request

```shell
curl "https://carikotak.com/register"
  -X "POST"
```

> Success Response

```shell
{
  "status": "created",
  "message": "account has been created",
  "url": "http://carikotak.com"
}
```

> Failed Response

```shell
{
  "status": "failed"
  "message": "account cannot be created"
}
```

This endpoint to register new user

#### HTTP REQUEST
`POST http://carikotak.com/register`

#### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
usename | required | username for credential
name | required | User name
email | required | User email address
password | required | User password

## Login to account

> Sample Request

```shell
curl "https://carikotak.com/login"
  -X "POST"
```

> Success Response

```shell
{
  "status": "logged",
  "message": "login sucess",
  "url": "http://carikotak.com"
}
```

> Failed Response

```shell
{
  "status": "unauthorized"
}
```

This endpoint to loggin to existing user account

#### HTTP REQUEST
`POST http://carikotak.com/login

#### PARAMETERS
Parameter |   | Description
--------- | ------- | -----------
username | required | Can be username or email address
password | required | User password

## Get API token

> Sample Request

```shell
curl "https://carikotak.com/oauth/token"
  -X "POST"
  -h "Accept        : application/json"
     "X-CSRF-TOKEN  : csrf_token"
     "x-Requested-With: XMLHttpRequest"
     "cache-control : no-cache"
```

> Success Response

```shell
{
  "token_type": "Bearer",
  "expires_in": 1295999,
  "access_token": "some_access_token",
  "refresh_token": "some_refresh_token"
}
```

This endpoint to get API token

#### HTTP REQUEST
`POST http://carikotak.com/oauth/token`

#### PARAMETERS
Parameter |  | Description
--------- | ------- | -----------
client_id | required | Oauth Client ID
client_secret | required | Oauth Client Secret
grant_type | required | 'password'
username | required | Can be username or email address
password | required | User password

## Social Auth

Login with Google or Facebook account

> Sample Request

```shell

curl "https://carikotak.com/social"
-X "POST"
-h "Accept        : application/json"
    "X-CSRF-TOKEN  : csrf_token"
    "x-Requested-With: XMLHttpRequest"
    "cache-control : no-cache"

```

> Success Response

```shell
{
  "status": "ok",
  "message": "login success",
  "url": "/"
}
```

This endpoint is used to authenticated with Facebook or Google Account

#### HTTP Request

`POST https://carikotak.com/social`

#### Parameters

Parameter |  | Description
--------- | ------- | -----------
name  | required  | Account name
email | required  | Account email
provider  | required | 'facebook' or 'google'
social_id | required | Account ID
avatar  | optional | Account Profile Picture