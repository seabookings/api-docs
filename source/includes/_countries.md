# Countries

## Get all countries and cities
```shell
curl "http://www.seabookings.com/api/v1/countries"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/countries", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
  "data": [
    {
      "id": "PT",
      "type": "country",
      "attributes": {
        "code": "PT",
        "cities": [
          {
            "name": "Benagil",
            "slug": "benagil"
          },
          {
            "name": "Abrantes",
            "slug": "abrantes"
          }
        ],
        "name": "Portugal",
        "details": {
          "country_data_or_code": "PT",
          "data": {
            "continent": "Europe",
            "address_format": "{{recipient}}\n{{street}}\n{{postalcode}} {{city}} {{region_short}}\n{{country}}",
            "alpha2": "PT",
            "alpha3": "PRT",
            "country_code": "351",
            "international_prefix": "00",
            "ioc": "POR",
            "gec": "PO",
            "name": "Portugal",
            "national_destination_code_lengths": [
              2
            ],
            "national_number_lengths": [
              9
            ],
            "national_prefix": "None",
            "number": "620",
            "region": "Europe",
            "subregion": "Southern Europe",
            "world_region": "EMEA",
            "un_locode": "PT",
            "nationality": "Portuguese",
            "eu_member": true,
            "eea_member": true,
            "vat_rates": {
              "standard": 23,
              "reduced": [
                6,
                13
              ],
              "super_reduced": null,
              "parking": 13
            },
            "postal_code": true,
            "unofficial_names": [
              "Portugal",
              "ポルトガル"
            ],
            "languages_official": [
              "pt"
            ],
            "languages_spoken": [
              "pt"
            ],
            "geo": {
              "latitude": 39.39987199999999,
              "latitude_dec": "39.64200973510742",
              "longitude": -8.224454,
              "longitude_dec": "-8.009422302246094",
              "max_latitude": 42.1542048,
              "max_longitude": -6.1902091,
              "min_latitude": 32.2895,
              "min_longitude": -31.4647999,
              "bounds": {
                "northeast": {
                  "lat": 42.1542048,
                  "lng": -6.1902091
                },
                "southwest": {
                  "lat": 32.2895,
                  "lng": -31.4647999
                }
              }
            },
            "currency_code": "EUR",
            "start_of_week": "monday",
            "translations": {
              "en": "Portugal",
              "pt": "Portugal",
              "es": "Portugal",
              "nl": "Portugal",
              "fr": "Portugal",
              "de": "Portugal"
            },
            "translated_names": [
              "Portugal",
              "Portugal",
              "Portugal",
              "Portugal",
              "Portugal",
              "Portugal"
            ]
          }
        }
      }
    }
  ]
}
```

### HTTP Request
`GET http://www.seabookings.com/api/v1/countries`
