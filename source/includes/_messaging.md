# Messaging

## Channel List

> Sample Request

```shell
curl "https://carikotak.com/api/channel"
  -X "GET"
```

Get All Channel User Joined

#### HTTP REQUEST
- `GET https://carikotak.com/channel`

## Read Channel

> Sample Request

```shell
curl "https://carikotak.com/api/channel/15"
  -X "GET"
```

Get All Message From a Channel User Joined

#### HTTP REQUEST
- `GET https://carikotak.com/channel/{channel_id}`

## Create Channel

> Sample Request

```shell
curl "https://carikotak.com/api/channel"
  -X "POST"
```

Create a new Channel with a User.
IF channel already exist, then return existing channel

#### HTTP REQUEST
- `POST https://carikotak.com/channel`

#### PARAMETERS
Parameter | Type  | Description
--------| ----- | -----------
name    | required  | Channel name
user_id | required  | Target user ID who want to invited to join a channel

## Delete Channel

> Sample Request

```shell
curl "https://carikotak.com/api/channel/15"
  -X "DELETE"
```

Remove User From Channel

#### HTTP REQUEST
- `DELETE https://carikotak.com/channel/{channel_id}`


## Send Message

> Sample Request

```shell
curl "https://carikotak.com/api/message"
  -X "POST"
```

Send Message in Joined Channel

#### HTTP REQUEST
- `POST https://carikotak.com/api/message`

#### PARAMETERS
Parameter | Type  | Description
--------| ----- | -----------
user_id  | required  | id of recepient user
message | required  | Message text

## Delete Message

> Sample Request

```shell
curl "https://carikotak.com/api/message/234"
  -X "DELETE"
```

Remove Message from Channel

#### HTTP REQUEST
- `DELETE https://carikotak.com/message/{message_id}`