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
      "id": "2",
      "type": "destination",
      "attributes": {
        "id": 2,
        "name": "Alvor",
        "short_description": "Alvor is one of our favorite seaside resorts of the Algarve, Southern Portugal. This fishing village is very pretty and continues to be rather authentic. ",
        "description": "<div>Alvor is one of our favorite seaside resorts of the Algarve, Southern Portugal. This fishing village is very pretty and continues to be rather authentic. Alvor is surrounded by some of the Algarve\u2019s finest beaches and golf courses.&nbsp;<\/div><div>Alvor has a distinctively Portuguese appearance with traditional whitewashed small houses, narrow streets and small fishing boats pulled up along the banks of the river. In the old town, the typical cobbled lanes lead down to the paved riverfront. Here you can find some of the freshest fish you\u2019ll ever eat.&nbsp;<\/div><div>Alvor is known for some of the most authentic sea experiences. It\u2019s historical ties make it a good option for the ones looking for a fishing boat tour. There are several options for boat tours in Alvor. For watersport lovers, the estuary of the river is very popular among kite and wind surfers.<\/div><div><br><\/div><ul><li>Our favorite beach: Praia dos Tr\u00eas Irm\u00e3os<\/li><li>Our favorite restaurant: Z\u00e9 Morgadinho<\/li><li>Our favorite boat tours in Alvor: Bottom fishing in Alvor<\/li><li>Our favorite water sport in Alvor: Fun boat tour in Alvor with snorkeling<\/li><\/ul>",
        "slug": "2-alvor",
        "total_activities": 11,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/42-shrine-s320181207-4-1brspjk-1544175285.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/42-shrine-s320181207-4-1brspjk-1544175285.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/42-shrine-s320181207-4-1brspjk-1544175285.jpg"
        },
        "country": {
          "name": "Portugal",
          "slug": "portugal",
          "code": "PT"
        }
      },
      "relationships": {
        "activities": {
          "data": [
            {
              "id": "112",
              "type": "activity"
            },
            {
              "id": "111",
              "type": "activity"
            },
            {
              "id": "482",
              "type": "activity"
            },
            {
              "id": "108",
              "type": "activity"
            },
            {
              "id": "188",
              "type": "activity"
            },
            {
              "id": "481",
              "type": "activity"
            },
            {
              "id": "189",
              "type": "activity"
            },
            {
              "id": "110",
              "type": "activity"
            },
            {
              "id": "187",
              "type": "activity"
            },
            {
              "id": "109",
              "type": "activity"
            },
            {
              "id": "113",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "5",
      "type": "destination",
      "attributes": {
        "id": 5,
        "name": "Arma\u00e7\u00e3o de P\u00eara",
        "short_description": "Arma\u00e7\u00e3o de P\u00eara is a small village very much focussed on tourism. Like most villages in the Algarve, Arma\u00e7\u00e3o de P\u00eara has a very laid back atmosphere.",
        "description": "<div>Arma\u00e7\u00e3o de P\u00eara is a small village very much focussed on tourism. Like most villages in the Algarve, Arma\u00e7\u00e3o de P\u00eara has a very laid back atmosphere. In the city center, you\u2019ll find a broad choice of bars and restaurants where the locals really make you feel welcome.&nbsp;<\/div><div>Arma\u00e7\u00e3o de P\u00eara is a good option if you\u2019re looking for some quiet holidays, specially during low season. From the lovely beach of Arma\u00e7\u00e3o, you can do several water sports and boat trips. You can\u2019t skip the boat tours in Arma\u00e7\u00e3o de P\u00eara to visit the famous Benagil cave.&nbsp;<\/div><div>For us, one of the downsides of Arma\u00e7\u00e3o de P\u00eara are it\u2019s tall buildings that strive above the cute authentic white houses and cobbled lanes.<\/div><div><br><\/div><ul><li>Our favorite beach: Praia de Albandeira<\/li><li>Our favorite restaurant: L'Oasis Pizzeria Italiana<\/li><li>Our favorite boat tour in Arma\u00e7\u00e3o de Pera: Boat trip to Benagil from Arma\u00e7\u00e3o de P\u00eara<\/li><li>Our favorite water sport in Arma\u00e7\u00e3o de P\u00eara: Kayak tour in Arma\u00e7\u00e3o de P\u00eara<\/li><\/ul>",
        "slug": "5-armacao-de-pera",
        "total_activities": 16,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/45-shrine-s320181207-4-1tzq2tg-1544175503.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/45-shrine-s320181207-4-1tzq2tg-1544175503.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/45-shrine-s320181207-4-1tzq2tg-1544175503.jpg"
        },
        "country": {
          "name": "Portugal",
          "slug": "portugal",
          "code": "PT"
        }
      },
      "relationships": {
        "activities": {
          "data": [
            {
              "id": "195",
              "type": "activity"
            },
            {
              "id": "197",
              "type": "activity"
            },
            {
              "id": "392",
              "type": "activity"
            },
            {
              "id": "134",
              "type": "activity"
            },
            {
              "id": "50",
              "type": "activity"
            },
            {
              "id": "198",
              "type": "activity"
            },
            {
              "id": "443",
              "type": "activity"
            },
            {
              "id": "212",
              "type": "activity"
            },
            {
              "id": "133",
              "type": "activity"
            },
            {
              "id": "136",
              "type": "activity"
            },
            {
              "id": "49",
              "type": "activity"
            },
            {
              "id": "52",
              "type": "activity"
            },
            {
              "id": "196",
              "type": "activity"
            },
            {
              "id": "137",
              "type": "activity"
            },
            {
              "id": "199",
              "type": "activity"
            },
            {
              "id": "135",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "6",
      "type": "destination",
      "attributes": {
        "id": 6,
        "name": "Aveiro",
        "short_description": "Aveiro is also known as the Venice of Portugal due to its channels that flow through the city. ",
        "description": "<div>Aveiro is also known as the Venice of Portugal due to its channels that flow through the city. You can hop aboard of a <em>moliceiro<\/em>, the famous boat tours in Aveiro through the channels and admire the colourful facades of the typical Portuguese houses. It\u2019s vibrant colors reflect the young and fun spirit of Aveiro.&nbsp;<\/div><div>In Aveiro, you find both historic buildings and modern architecture, as well as beautiful beaches. You can cruise through the city on a boat tour or by foot while enjoying \u201cOvos Moles\u201d, a special dessert that you can only find in this city.<\/div><div>If you are a fan of the real feel while traveling, get aboard on one of our boat tours in Aveiro and be amazed by the beautiful views.&nbsp;<\/div><div><br><\/div><ul><li>Our favorite beach: Praia do Furadouro<\/li><li>Our favorite restaurant: Culpa da Vontade<\/li><li>Our favorite boat tour in Aveiro: Full day fishing tour in Aveiro<\/li><\/ul>",
        "slug": "6-aveiro",
        "total_activities": 4,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/46-shrine-s320181207-4-1p98tjy-1544175558.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/46-shrine-s320181207-4-1p98tjy-1544175558.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/46-shrine-s320181207-4-1p98tjy-1544175558.jpg"
        },
        "country": {
          "name": "Portugal",
          "slug": "portugal",
          "code": "PT"
        }
      },
      "relationships": {
        "activities": {
          "data": [
            {
              "id": "164",
              "type": "activity"
            },
            {
              "id": "163",
              "type": "activity"
            },
            {
              "id": "161",
              "type": "activity"
            },
            {
              "id": "162",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "3",
      "type": "destination",
      "attributes": {
        "id": 3,
        "name": "Alicante",
        "short_description": "Alicante is one of the hot-spots when it comes to tourism on the Spanish mainland! No wonder, because Alicante has a lot to offer.",
        "description": "<div>Alicante is one of the hot-spots when it comes to tourism on the Spanish mainland! No wonder, because Alicante has a lot to offer. Whether you are looking for beautiful white-sanded beaches, rich culture with museums, delicious food, sightseeing or a busy nightlife - you find it all in Alicante!&nbsp;<\/div><div>Situated right on the Mediterranean Sea, the water in Alicante is calm and warm, inviting you to do some of the many watersport activities offered along the coast of Alicante. The beaches are some of the best in Spain, and if you wish to have a delicious Paella after a beach day, just head into the little centre and you\u2019ll find enough options! At \u201cEl Barrio\u201d you can continue having fun in one of the numerous bars and clubs!&nbsp;<\/div><div><br><\/div><ul><li>Our favorite beach: San Juan de Alicante&nbsp;<\/li><li>Our favorite restaurant: Don Carlos Alicante<\/li><li>Our favorite boat tours in Alicante: Full day catamaran boat tour in Alicante<\/li><li>Our favorite water sport in Alicante: Kayak tour in Alicante with snorkeling<\/li><\/ul>",
        "slug": "3-alicante",
        "total_activities": 12,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/43-shrine20181211-97273-1qpkflj-1544546380.jpeg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/43-shrine20181211-97273-1qpkflj-1544546380.jpeg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/43-shrine20181211-97273-1qpkflj-1544546380.jpeg"
        },
        "country": {
          "name": "Spain",
          "slug": "spain",
          "code": "ES"
        }
      },
      "relationships": {
        "activities": {
          "data": [
            {
              "id": "337",
              "type": "activity"
            },
            {
              "id": "316",
              "type": "activity"
            },
            {
              "id": "259",
              "type": "activity"
            },
            {
              "id": "260",
              "type": "activity"
            },
            {
              "id": "278",
              "type": "activity"
            },
            {
              "id": "340",
              "type": "activity"
            },
            {
              "id": "338",
              "type": "activity"
            },
            {
              "id": "277",
              "type": "activity"
            },
            {
              "id": "341",
              "type": "activity"
            },
            {
              "id": "261",
              "type": "activity"
            },
            {
              "id": "336",
              "type": "activity"
            },
            {
              "id": "339",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "4",
      "type": "destination",
      "attributes": {
        "id": 4,
        "name": "Almer\u00eda",
        "short_description": "This sunny city in Andaluc\u00eda has been becoming more and more popular among travellers.",
        "description": "<div>This sunny city in Andaluc\u00eda has been becoming more and more popular among travellers. The historic old town with its little streets, the impressive fortress and the cute port make for some great photos and invite you to discover all the different sides Almer\u00eda has to offer.&nbsp;<\/div><div>While the city is lively with many options to eat and drink and of course relax at the beach, you can also choose to head a little east and visit the amazing natural park Cabo da Gata - N\u00edjar. Here you can find wild volcanic landscapes, hidden coves and so much untouched nature that you will feel like in a different world! And after getting back to the cultural centre of Almer\u00eda, why not reward yourself with some of the delicious seafood of the region!<\/div><div><br><\/div><ul><li>Our favorite beach: Aguadulce beach<\/li><li>Our favorite restaurant: La Gruta<\/li><li>Our favorite water sport in Almer\u00eda: Kayak tour in Almer\u00eda<\/li><\/ul>",
        "slug": "4-almeria",
        "total_activities": 6,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/44-shrine20181211-97273-1niron6-1544546403.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/44-shrine20181211-97273-1niron6-1544546403.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/44-shrine20181211-97273-1niron6-1544546403.jpg"
        },
        "country": {
          "name": "Spain",
          "slug": "spain",
          "code": "ES"
        }
      },
      "relationships": {
        "activities": {
          "data": [
            {
              "id": "606",
              "type": "activity"
            },
            {
              "id": "354",
              "type": "activity"
            },
            {
              "id": "602",
              "type": "activity"
            },
            {
              "id": "360",
              "type": "activity"
            },
            {
              "id": "618",
              "type": "activity"
            },
            {
              "id": "267",
              "type": "activity"
            }
          ]
        }
      }
    }
  ]
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/destinations`

### Query Parameters

Parameter    | Default | Description
------------ | ------- | -----------
featured     | false   | If you just want the featured desinations or all
country_code | null    | If you want the destinations associated with a specific country. If none are specified destinations for all countries are returned.
include      | null    | Allows you to sideload associations. Allowed value `activities`


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
    "id": "5",
    "type": "destination",
    "attributes": {
      "id": 5,
      "name": "Arma\u00e7\u00e3o de P\u00eara",
      "short_description": "Arma\u00e7\u00e3o de P\u00eara is a small village very much focussed on tourism. Like most villages in the Algarve, Arma\u00e7\u00e3o de P\u00eara has a very laid back atmosphere.",
      "description": "<div>Arma\u00e7\u00e3o de P\u00eara is a small village very much focussed on tourism. Like most villages in the Algarve, Arma\u00e7\u00e3o de P\u00eara has a very laid back atmosphere. In the city center, you\u2019ll find a broad choice of bars and restaurants where the locals really make you feel welcome.&nbsp;<\/div><div>Arma\u00e7\u00e3o de P\u00eara is a good option if you\u2019re looking for some quiet holidays, specially during low season. From the lovely beach of Arma\u00e7\u00e3o, you can do several water sports and boat trips. You can\u2019t skip the boat tours in Arma\u00e7\u00e3o de P\u00eara to visit the famous Benagil cave.&nbsp;<\/div><div>For us, one of the downsides of Arma\u00e7\u00e3o de P\u00eara are it\u2019s tall buildings that strive above the cute authentic white houses and cobbled lanes.<\/div><div><br><\/div><ul><li>Our favorite beach: Praia de Albandeira<\/li><li>Our favorite restaurant: L'Oasis Pizzeria Italiana<\/li><li>Our favorite boat tour in Arma\u00e7\u00e3o de Pera: Boat trip to Benagil from Arma\u00e7\u00e3o de P\u00eara<\/li><li>Our favorite water sport in Arma\u00e7\u00e3o de P\u00eara: Kayak tour in Arma\u00e7\u00e3o de P\u00eara<\/li><\/ul>",
      "slug": "5-armacao-de-pera",
      "total_activities": 16,
      "media": {
        "original": "http:\/\/app.sb.com:3000\/photos\/original\/45-shrine-s320181207-4-1tzq2tg-1544175503.jpg",
        "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/45-shrine-s320181207-4-1tzq2tg-1544175503.jpg",
        "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/45-shrine-s320181207-4-1tzq2tg-1544175503.jpg"
      },
      "country": {
        "name": "Portugal",
        "slug": "portugal",
        "code": "PT"
      }
    },
    "relationships": {
      "activities": {
        "data": [
          {
            "id": "195",
            "type": "activity"
          },
          {
            "id": "197",
            "type": "activity"
          },
          {
            "id": "392",
            "type": "activity"
          },
          {
            "id": "134",
            "type": "activity"
          },
          {
            "id": "50",
            "type": "activity"
          },
          {
            "id": "198",
            "type": "activity"
          },
          {
            "id": "443",
            "type": "activity"
          },
          {
            "id": "212",
            "type": "activity"
          },
          {
            "id": "133",
            "type": "activity"
          },
          {
            "id": "136",
            "type": "activity"
          },
          {
            "id": "49",
            "type": "activity"
          },
          {
            "id": "52",
            "type": "activity"
          },
          {
            "id": "196",
            "type": "activity"
          },
          {
            "id": "137",
            "type": "activity"
          },
          {
            "id": "199",
            "type": "activity"
          },
          {
            "id": "135",
            "type": "activity"
          }
        ]
      }
    }
  }
}
```

### HTTP Request

`GET https://api.seabookings.com/api/v1/destination/5-armacao-de-pera`



Parameter    | Default | Description
------------ | ------- | -----------
include      | null    | Allows you to sideload associations. Allowed value `activities`
