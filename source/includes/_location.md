# Location

## Get All Provinces

> Sample Request

```shell
    
curl "https://carikotak.com/api/location?get=provinces"
  -X "GET"

```

#### HTTP REQUEST
- `GET https://carikotak.com/api/location?get=provinces`

## Get All Cities

> Sample Request

```shell
    
curl "https://carikotak.com/api/location?get=cities"
  -X "GET"

```

#### HTTP REQUEST
- `GET https://carikotak.com/api/location?get=cities`

## Get All Cities from a Province

> Sample Request

```shell
    
curl "https://carikotak.com/api/location?get=cities&from=11"
  -X "GET"

```

#### HTTP REQUEST
- `GET https://carikotak.com/api/location?get=cities&from={province_id}`

## Get All Cities from all Provinces

> Sample Request

```shell
    
curl "https://carikotak.com/api/location?get=provinces&with=cities"
  -X "GET"

```

#### HTTP REQUEST
- `GET https://carikotak.com/api/location?get=provinces&with=cities`