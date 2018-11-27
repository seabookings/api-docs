# Destinations

Destinations comprehends a set of locations that are featured in the seabookings portal.

## Get destinations

```shell
curl "https://api.seabookings.com/api/v1/destinations"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/destinations" ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            "id": "1",
            "type": "destination",
            "attributes": {
                "id": 1,
                "name": "Algarve",
                "short_description": "Short description for Algarve",
                "description": "<div>Long description for Algarve</div>",
                "slug": "1-algarve",
                "media": {
                    "original": "https://api.seabookings.com/photos/original/41-faro-boat-tour-1543257148.jpg",
                    "thumbnail": "https://api.seabookings.com/photos/thumbnail/41-faro-boat-tour-1543257148.jpg",
                    "medium": "https://api.seabookings.com/photos/medium/41-faro-boat-tour-1543257148.jpg"
                },
                "country": {
                    "name": "Portugal",
                    "slug": "portugal",
                    "code": "PT"
                },
                "cities": [
                    {
                        "name": "Albufeira",
                        "slug": "albufeira"
                    },
                    {
                        "name": "Lagos",
                        "slug": "lagos"
                    },
                    {
                        "name": "Vilamoura",
                        "slug": "vilamoura"
                    }
                ]
            }
        },
        {
            "id": "2",
            "type": "destination",
            "attributes": {
                "id": 2,
                "name": "Lisbon",
                "short_description": "Short description for Lisbon",
                "description": "<div>Long description for Lisbon</div>",
                "slug": "2-lisbon",
                "media": {
                    "original": "https://api.seabookings.com/photos/original/42-shrine20181126-44259-9fpbjf-1543257120.jpg",
                    "thumbnail": "https://api.seabookings.com/photos/thumbnail/42-shrine20181126-44259-9fpbjf-1543257120.jpg",
                    "medium": "https://api.seabookings.com/photos/medium/42-shrine20181126-44259-9fpbjf-1543257120.jpg"
                },
                "country": {
                    "name": "Portugal",
                    "slug": "portugal",
                    "code": "PT"
                },
                "cities": [
                    {
                        "name": "Cascais",
                        "slug": "cascais"
                    },
                    {
                        "name": "Lisboa",
                        "slug": "lisboa"
                    }
                ]
            }
        }
    ]
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/destinations`




## Get destination

```shell
curl "https://api.seabookings.com/api/v1/destinations/1-algarve"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/destination/1-algarve" ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": "1",
        "type": "destination",
        "attributes": {
            "id": 1,
            "name": "Algarve",
            "short_description": "Short description for Algarve",
            "description": "<div>Long description for Algarve</div>",
            "slug": "1-algarve",
            "media": {
                "original": "https://api.seabookings.com/photos/original/41-faro-boat-tour-1543257148.jpg",
                "thumbnail": "https://api.seabookings.com/photos/thumbnail/41-faro-boat-tour-1543257148.jpg",
                "medium": "https://api.seabookings.com/photos/medium/41-faro-boat-tour-1543257148.jpg"
            },
            "country": {
                "name": "Portugal",
                "slug": "portugal",
                "code": "PT"
            },
            "cities": [
                {
                    "name": "Albufeira",
                    "slug": "albufeira"
                },
                {
                    "name": "Lagos",
                    "slug": "lagos"
                },
                {
                    "name": "Vilamoura",
                    "slug": "vilamoura"
                }
            ]
        }
    }
}
```

### HTTP Request

`GET https://api.seabookings.com/api/v1/destination/1-algarve`



