# Rating

## Give Rating or Update Rating

> Sample Request

```shell
curl "https://carikotak.com/api/rating"
  -X "POST"
```

#### HTTP REQUEST
- `POST https://carikotak.com/api/rating`

#### PARAMETERS

Parameter   | Type  | Description
--------| ----- | -----------
target_id   | required  | product or post id
target_type | required  | 'product' or 'post' default 'product'
rating      | required  | rating float number 0 to 5