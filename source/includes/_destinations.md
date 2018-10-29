# Destinations

Destinations comprehends a set of locations that are featured in the seabookings portal.

## Get destinations

```shell
curl "http://www.seabookings.com/api/v1/destinations"
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
                "name": "jj",
                "short_description": "xpto",
                "description": "<div>xpto</div>",
                "cover_photo": "/uploads/destination/1/cover_photo/original-8efc3225b691d20b899ae1f9df782abd.jpg",
                "country": {
                    "name": "Portugal",
                    "slug": "portugal",
                    "code": "PT"
                },
                "cities": [
                    {
                        "name": "Abrantes",
                        "slug": "abrantes"
                    },
                    {
                        "name": "Lisbon",
                        "slug": "lisbon"
                    }
                ]
            }
        },
        {
            "id": "2",
            "type": "destination",
            "attributes": {
                "id": 2,
                "name": "Things to do in madeira",
                "short_description": "Madeira, an island you can forget. Watch the dolphins and whales on this green paradise",
                "description": "<div>Madeira is a perfect holiday destination the whole year round. We’ll share the some tips to take the most out of your holidays on the island and enjoy the best things to do on Madeira.<br><br></div><div>Madeira is one of the archipelagos of Portugal. The archipelago is composed by two inhabited islands, Madeira and Porto Santo, and a few islands where no people live on. The capital of this autonomous region is Funchal.<br><br></div><div>The islands of <a href=\"https://www.seabookings.com/things-to-do-in-portugal/madeira/\">Madeira</a> and Porto Santo are characterized by a warm subtropical climate all year round. Madeira is very popular for active travellers who like outdoor experiences like hiking or <a href=\"http://www.runinportugal.com/\">running in the mountains</a>, playing golf or water activities like <a href=\"https://www.seabookings.com/package/surf-on-madeira-island/\">surf</a>, <a href=\"https://www.seabookings.com/package/sup-on-madeira-island/\">SUP</a>, kayak and <a href=\"https://www.seabookings.com/things-to-do-in-portugal/madeira/\">boat tours</a>.<br><br></div>",
                "cover_photo": "/uploads/destination/2/cover_photo/original-3d665161e5f7f72b3b31fe870fece675.jpg",
                "country": {
                    "name": "Portugal",
                    "slug": "portugal",
                    "code": "PT"
                },
                "cities": []
            }
        }
    ]
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/destinations`

