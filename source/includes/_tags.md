# Tags

## Get all tags

```shell
curl "http://www.seabookings.com/api/v1/tags"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/tags"); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            "id": "1",
            "type": "tag",
            "attributes": {
                "id": 1,
                "key": "family",
                "label": "Family friendly"
            }
        },
        {
            "id": "2",
            "type": "tag",
            "attributes": {
                "id": 2,
                "key": "dolphins",
                "label": "Dolphin watching"
            }
        },
        {
            "id": "3",
            "type": "tag",
            "attributes": {
                "id": 3,
                "key": "whales",
                "label": "Whale watching"
            }
        },
        {
            "id": "4",
            "type": "tag",
            "attributes": {
                "id": 4,
                "key": "exciting",
                "label": "Exciting"
            }
        },
        {
            "id": "5",
            "type": "tag",
            "attributes": {
                "id": 5,
                "key": "groups",
                "label": "Groups friendly"
            }
        },
        {
            "id": "6",
            "type": "tag",
            "attributes": {
                "id": 6,
                "key": "jet_ski",
                "label": "Jet ski"
            }
        },
        {
            "id": "7",
            "type": "tag",
            "attributes": {
                "id": 7,
                "key": "sailing",
                "label": "Sailing tours"
            }
        },
        {
            "id": "8",
            "type": "tag",
            "attributes": {
                "id": 8,
                "key": "diving",
                "label": "Diving"
            }
        },
        {
            "id": "9",
            "type": "tag",
            "attributes": {
                "id": 9,
                "key": "fishing",
                "label": "Fishing"
            }
        },
        {
            "id": "10",
            "type": "tag",
            "attributes": {
                "id": 10,
                "key": "pregnant_safe",
                "label": "Pregnant safe"
            }
        },
        {
            "id": "11",
            "type": "tag",
            "attributes": {
                "id": 11,
                "key": "accessible",
                "label": "Accessible"
            }
        },
        {
            "id": "12",
            "type": "tag",
            "attributes": {
                "id": 12,
                "key": "children_safe",
                "label": "Children safe"
            }
        },
        {
            "id": "13",
            "type": "tag",
            "attributes": {
                "id": 13,
                "key": "party_boat",
                "label": "Party boat"
            }
        },
        {
            "id": "14",
            "type": "tag",
            "attributes": {
                "id": 14,
                "key": "romantic",
                "label": "Romantic tours"
            }
        },
        {
            "id": "15",
            "type": "tag",
            "attributes": {
                "id": 15,
                "key": "kayak",
                "label": "Kayak tours"
            }
        },
        {
            "id": "16",
            "type": "tag",
            "attributes": {
                "id": 16,
                "key": "speedboat",
                "label": "Speed boat tours"
            }
        },
        {
            "id": "17",
            "type": "tag",
            "attributes": {
                "id": 17,
                "key": "snorkeling",
                "label": "Snorkeling"
            }
        },
        {
            "id": "18",
            "type": "tag",
            "attributes": {
                "id": 18,
                "key": "sunset",
                "label": "Sunset tours"
            }
        },
        {
            "id": "19",
            "type": "tag",
            "attributes": {
                "id": 19,
                "key": "surf",
                "label": "Surf"
            }
        }
    ]
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/tags`

