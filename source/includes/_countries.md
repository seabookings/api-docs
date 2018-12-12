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
      "id": "1",
      "type": "country",
      "attributes": {
        "code": "PT",
        "name": "Portugal",
        "slug": "portugal",
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
              "\u30dd\u30eb\u30c8\u30ac\u30eb"
            ],
            "languages_official": [
              "pt"
            ],
            "languages_spoken": [
              "pt"
            ],
            "geo": {
              "latitude": 39.399872,
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
        },
        "flag": "\/assets\/flags\/pt-e8768374a06ad93246ee0bcf798116ac26e68ad44732aeb02e6536b46f72dbe7.png"
      },
      "relationships": {
        "destinations": {
          "data": [
            {
              "id": "2",
              "type": "destination"
            },
            {
              "id": "5",
              "type": "destination"
            },
            {
              "id": "6",
              "type": "destination"
            },
            {
              "id": "9",
              "type": "destination"
            },
            {
              "id": "7",
              "type": "destination"
            },
            {
              "id": "12",
              "type": "destination"
            },
            {
              "id": "19",
              "type": "destination"
            },
            {
              "id": "20",
              "type": "destination"
            },
            {
              "id": "15",
              "type": "destination"
            },
            {
              "id": "27",
              "type": "destination"
            },
            {
              "id": "22",
              "type": "destination"
            },
            {
              "id": "23",
              "type": "destination"
            },
            {
              "id": "24",
              "type": "destination"
            },
            {
              "id": "25",
              "type": "destination"
            },
            {
              "id": "28",
              "type": "destination"
            },
            {
              "id": "31",
              "type": "destination"
            },
            {
              "id": "34",
              "type": "destination"
            },
            {
              "id": "1",
              "type": "destination"
            }
          ]
        }
      }
    },
    {
      "id": "2",
      "type": "country",
      "attributes": {
        "code": "AE",
        "name": "United Arab Emirates",
        "slug": "united-arab-emirates",
        "details": {
          "country_data_or_code": "AE",
          "data": {
            "continent": "Asia",
            "address_format": "{{recipient}}\n{{street}}\n{{postalcode}} {{city}}\n{{country}}",
            "alpha2": "AE",
            "alpha3": "ARE",
            "country_code": "971",
            "international_prefix": "00",
            "ioc": "UAE",
            "gec": "AE",
            "name": "United Arab Emirates",
            "national_destination_code_lengths": [
              2
            ],
            "national_number_lengths": [
              7,
              8,
              9
            ],
            "national_prefix": "0",
            "number": "784",
            "region": "Asia",
            "subregion": "Western Asia",
            "world_region": "EMEA",
            "un_locode": "AE",
            "nationality": "Emirian",
            "postal_code": false,
            "unofficial_names": [
              "United Arab Emirates",
              "\u0627\u0644\u0625\u0645\u0627\u0631\u0627\u062a \u0627\u0644\u0639\u0631\u0628\u064a\u0629 \u0627\u0644\u0645\u062a\u062d\u062f\u0629",
              "Vereinigte Arabische Emirate",
              "\u00c9mirats Arabes Unis",
              "Emiratos \u00c1rabes Unidos",
              "\u30a2\u30e9\u30d6\u9996\u9577\u56fd\u9023\u90a6",
              "Verenigde Arabische Emiraten"
            ],
            "languages_official": [
              "ar"
            ],
            "languages_spoken": [
              "ar"
            ],
            "geo": {
              "latitude": 23.424076,
              "latitude_dec": "23.684776306152344",
              "longitude": 53.847818,
              "longitude_dec": "54.536643981933594",
              "max_latitude": 26.0765,
              "max_longitude": 56.4395001,
              "min_latitude": 22.6315138,
              "min_longitude": 51.4723,
              "bounds": {
                "northeast": {
                  "lat": 26.0765,
                  "lng": 56.4395001
                },
                "southwest": {
                  "lat": 22.6315138,
                  "lng": 51.4723
                }
              }
            },
            "currency_code": "AED",
            "start_of_week": "sunday",
            "translations": {
              "en": "United Arab Emirates",
              "pt": "Emirados \u00c1rabes Unidos",
              "es": "Emiratos \u00c1rabes Unidos",
              "nl": "Verenigde Arabische Emiraten",
              "fr": "\u00c9mirats arabes unis",
              "de": "Vereinigte Arabische Emirate"
            },
            "translated_names": [
              "United Arab Emirates",
              "Emirados \u00c1rabes Unidos",
              "Emiratos \u00c1rabes Unidos",
              "Verenigde Arabische Emiraten",
              "\u00c9mirats arabes unis",
              "Vereinigte Arabische Emirate"
            ]
          }
        },
        "flag": "\/assets\/flags\/ae-4b37c19482652746a83d39f5ab99401590fab7fc611f5a1e173eec7240ae21aa.png"
      },
      "relationships": {
        "destinations": {
          "data": [
            {
              "id": "14",
              "type": "destination"
            }
          ]
        }
      }
    },
    {
      "id": "3",
      "type": "country",
      "attributes": {
        "code": "ES",
        "name": "Spain",
        "slug": "spain",
        "details": {
          "country_data_or_code": "ES",
          "data": {
            "continent": "Europe",
            "address_format": "{{recipient}}\n{{street}}\n{{postalcode}} {{city}}\n{{region}}\n{{country}}",
            "alpha2": "ES",
            "alpha3": "ESP",
            "country_code": "34",
            "international_prefix": "00",
            "ioc": "ESP",
            "gec": "SP",
            "name": "Spain",
            "national_destination_code_lengths": [
              2
            ],
            "national_number_lengths": [
              9
            ],
            "national_prefix": "None",
            "number": "724",
            "region": "Europe",
            "subregion": "Southern Europe",
            "world_region": "EMEA",
            "un_locode": "ES",
            "nationality": "Spanish",
            "eu_member": true,
            "eea_member": true,
            "vat_rates": {
              "standard": 21,
              "reduced": [
                10
              ],
              "super_reduced": 4,
              "parking": null
            },
            "postal_code": true,
            "unofficial_names": [
              "Spain",
              "Spanien",
              "Espagne",
              "Espa\u00f1a",
              "\u30b9\u30da\u30a4\u30f3",
              "Spanje"
            ],
            "languages_official": [
              "es"
            ],
            "languages_spoken": [
              "es"
            ],
            "geo": {
              "latitude": 40.463667,
              "latitude_dec": "40.396026611328125",
              "longitude": -3.74922,
              "longitude_dec": "-3.550692558288574",
              "max_latitude": 43.8504,
              "max_longitude": 4.6362,
              "min_latitude": 27.4985,
              "min_longitude": -18.2648001,
              "bounds": {
                "northeast": {
                  "lat": 43.8504,
                  "lng": 4.6362
                },
                "southwest": {
                  "lat": 27.4985,
                  "lng": -18.2648001
                }
              }
            },
            "currency_code": "EUR",
            "start_of_week": "monday",
            "translations": {
              "en": "Spain",
              "pt": "Espanha",
              "es": "Espa\u00f1a",
              "nl": "Spanje",
              "fr": "Espagne",
              "de": "Spanien"
            },
            "translated_names": [
              "Spain",
              "Espanha",
              "Espa\u00f1a",
              "Spanje",
              "Espagne",
              "Spanien"
            ]
          }
        },
        "flag": "\/assets\/flags\/es-011b2b93663e8954ee866aa017bfe21e4b0b94a6067035ed6851110b58b53fc7.png"
      },
      "relationships": {
        "destinations": {
          "data": [
            {
              "id": "3",
              "type": "destination"
            },
            {
              "id": "4",
              "type": "destination"
            },
            {
              "id": "10",
              "type": "destination"
            },
            {
              "id": "16",
              "type": "destination"
            },
            {
              "id": "18",
              "type": "destination"
            },
            {
              "id": "17",
              "type": "destination"
            },
            {
              "id": "21",
              "type": "destination"
            },
            {
              "id": "30",
              "type": "destination"
            },
            {
              "id": "32",
              "type": "destination"
            },
            {
              "id": "8",
              "type": "destination"
            }
          ]
        }
      }
    },
    {
      "id": "4",
      "type": "country",
      "attributes": {
        "code": "HR",
        "name": "Croatia",
        "slug": "croatia",
        "details": {
          "country_data_or_code": "HR",
          "data": {
            "continent": "Europe",
            "address_format": "{{recipient}}\n{{street}}\n{{postalcode}} {{city}}\n{{country}}",
            "alpha2": "HR",
            "alpha3": "HRV",
            "country_code": "385",
            "international_prefix": "00",
            "ioc": "CRO",
            "gec": "HR",
            "name": "Croatia",
            "national_destination_code_lengths": [
              2
            ],
            "national_number_lengths": [
              8
            ],
            "national_prefix": "0",
            "number": "191",
            "region": "Europe",
            "subregion": "Southern Europe",
            "world_region": "EMEA",
            "un_locode": "HR",
            "nationality": "Croatian",
            "eu_member": true,
            "eea_member": true,
            "vat_rates": {
              "standard": 25,
              "reduced": [
                5,
                13
              ],
              "super_reduced": null,
              "parking": null
            },
            "postal_code": true,
            "unofficial_names": [
              "Croatia",
              "Kroatien",
              "Croatie",
              "Croacia",
              "\u30af\u30ed\u30a2\u30c1\u30a2",
              "Kroati\u00eb",
              "Croatia (Hrvatska)"
            ],
            "languages_official": [
              "hr"
            ],
            "languages_spoken": [
              "hr"
            ],
            "geo": {
              "latitude": 45.1,
              "latitude_dec": "45.444305419921875",
              "longitude": 15.2,
              "longitude_dec": "15.734503746032715",
              "max_latitude": 46.5549857,
              "max_longitude": 19.4480523,
              "min_latitude": 42.3385087,
              "min_longitude": 13.3649,
              "bounds": {
                "northeast": {
                  "lat": 46.5549857,
                  "lng": 19.4480523
                },
                "southwest": {
                  "lat": 42.3385087,
                  "lng": 13.3649
                }
              }
            },
            "currency_code": "HRK",
            "start_of_week": "monday",
            "translations": {
              "en": "Croatia",
              "pt": "Cro\u00e1cia",
              "es": "Croacia",
              "nl": "Kroati\u00eb",
              "fr": "Croatie",
              "de": "Kroatien"
            },
            "translated_names": [
              "Croatia",
              "Cro\u00e1cia",
              "Croacia",
              "Kroati\u00eb",
              "Croatie",
              "Kroatien"
            ]
          }
        },
        "flag": "\/assets\/flags\/hr-ea140329ba2f75db6b1c322da25edb90bfe9b0b9b5d5d03eb7f550ecf711c066.png"
      },
      "relationships": {
        "destinations": {
          "data": [
            {
              "id": "29",
              "type": "destination"
            },
            {
              "id": "33",
              "type": "destination"
            }
          ]
        }
      }
    },
    {
      "id": "5",
      "type": "country",
      "attributes": {
        "code": "GR",
        "name": "Greece",
        "slug": "greece",
        "details": {
          "country_data_or_code": "GR",
          "data": {
            "continent": "Europe",
            "address_format": "{{recipient}}\n{{street}}\n{{postalcode}} {{city}}\n{{country}}",
            "alpha2": "GR",
            "alpha3": "GRC",
            "country_code": "30",
            "international_prefix": "00",
            "ioc": "GRE",
            "gec": "GR",
            "name": "Greece",
            "national_destination_code_lengths": [
              2
            ],
            "national_number_lengths": [
              10
            ],
            "national_prefix": "None",
            "number": "300",
            "region": "Europe",
            "subregion": "Southern Europe",
            "world_region": "EMEA",
            "un_locode": "GR",
            "nationality": "Greek",
            "eu_member": true,
            "eea_member": true,
            "vat_rates": {
              "standard": 23,
              "reduced": [
                6.5,
                13
              ],
              "super_reduced": null,
              "parking": null
            },
            "postal_code": true,
            "unofficial_names": [
              "Greece",
              "Griechenland",
              "Gr\u00e8ce",
              "Grecia",
              "\u30ae\u30ea\u30b7\u30e3",
              "Griekenland"
            ],
            "languages_official": [
              "el"
            ],
            "languages_spoken": [
              "el"
            ],
            "geo": {
              "latitude": 39.074208,
              "latitude_dec": "39.68437194824219",
              "longitude": 21.824312,
              "longitude_dec": "21.897409439086914",
              "max_latitude": 41.7488784,
              "max_longitude": 29.6527999,
              "min_latitude": 34.5428,
              "min_longitude": 19.3098,
              "bounds": {
                "northeast": {
                  "lat": 41.7488784,
                  "lng": 29.6527999
                },
                "southwest": {
                  "lat": 34.5428,
                  "lng": 19.3098
                }
              }
            },
            "currency_code": "EUR",
            "start_of_week": "monday",
            "translations": {
              "en": "Greece",
              "pt": "Gr\u00e9cia",
              "es": "Grecia",
              "nl": "Griekenland",
              "fr": "Gr\u00e8ce",
              "de": "Griechenland"
            },
            "translated_names": [
              "Greece",
              "Gr\u00e9cia",
              "Grecia",
              "Griekenland",
              "Gr\u00e8ce",
              "Griechenland"
            ]
          }
        },
        "flag": "\/assets\/flags\/gr-6877fc32271c9efedac5d8a844f4745a58344a307e0d19c687f82091e3a819b2.png"
      },
      "relationships": {
        "destinations": {
          "data": [
            {
              "id": "13",
              "type": "destination"
            },
            {
              "id": "26",
              "type": "destination"
            }
          ]
        }
      }
    },
    {
      "id": "6",
      "type": "country",
      "attributes": {
        "code": "CV",
        "name": "Cape Verde",
        "slug": "cape-verde",
        "details": {
          "country_data_or_code": "CV",
          "data": {
            "continent": "Africa",
            "alpha2": "CV",
            "alpha3": "CPV",
            "country_code": "238",
            "international_prefix": "00",
            "ioc": "CPV",
            "gec": "CV",
            "name": "Cabo Verde",
            "national_destination_code_lengths": [
              2
            ],
            "national_number_lengths": [
              7
            ],
            "national_prefix": "None",
            "number": "132",
            "region": "Africa",
            "subregion": "Western Africa",
            "world_region": "EMEA",
            "un_locode": "CV",
            "nationality": "Cape Verdian",
            "postal_code": true,
            "unofficial_names": [
              "Cape Verde",
              "Kap Verde",
              "Cap Vert",
              "Cabo Verde",
              "\u30ab\u30fc\u30dc\u30d9\u30eb\u30c7",
              "Kaapverdi\u00eb"
            ],
            "languages_official": [
              "pt"
            ],
            "languages_spoken": [
              "pt"
            ],
            "geo": {
              "latitude": 15.120142,
              "latitude_dec": "15.183002471923828",
              "longitude": -23.6051868,
              "longitude_dec": "-23.70345115661621",
              "max_latitude": 17.3191764,
              "max_longitude": -22.5933839,
              "min_latitude": 14.7270733,
              "min_longitude": -25.383911,
              "bounds": {
                "northeast": {
                  "lat": 17.3191764,
                  "lng": -22.5933839
                },
                "southwest": {
                  "lat": 14.7270733,
                  "lng": -25.383911
                }
              }
            },
            "currency_code": "CVE",
            "start_of_week": "monday",
            "translations": {
              "en": "Cape Verde",
              "pt": "Cabo Verde",
              "es": "Cabo Verde",
              "nl": "Kaapverdi\u00eb",
              "fr": "Cap-Vert",
              "de": "Cabo Verde"
            },
            "translated_names": [
              "Cape Verde",
              "Cabo Verde",
              "Cabo Verde",
              "Kaapverdi\u00eb",
              "Cap-Vert",
              "Cabo Verde"
            ]
          }
        },
        "flag": "\/flags\/cv.png"
      },
      "relationships": {
        "destinations": {
          "data": [
            {
              "id": "11",
              "type": "destination"
            }
          ]
        }
      }
    }
  ],
  "included": [
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
      "id": "9",
      "type": "destination",
      "attributes": {
        "id": 9,
        "name": "Benagil",
        "short_description": "Benagil is worldwide known for its famous grottos, that can only be accessed by sea.",
        "description": "<div>Benagil is a small and typical fishertown in the Algarve. Benagil is worldwide known for its famous grottos, that can only be accessed by sea. The Benagil caves are the most popular ones of all maritime caves in Portugal. A boat tour in Benagil is an unique and exciting way to discover these breathtaking grottos. And just next to Benagil Beach you can visit yet another paradisiacal beach called Praia da Marinha.&nbsp;<\/div><div>The boat tour in Benagil to visit the caves are an absolute Must-Do during holidays in the Algarve. It\u2019s an unforgettable experience that leaves you stunned and amazed by the beauty of nature. The coast around Benagil is also home to dolphins and whales, so if you prefer, you can even go on a two-in-one boat trip which takes you to the dolphins and the Benagil cave!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia de Benagil<\/li><li>Our favorite restaurant: O Pescador Benagil<\/li><li>Our favorite boat tour in Benagil: Discover the Benagil cave on a boat tour<\/li><li>Our favorite water sport in Benagil: SUP tour in Benagil<\/li><\/ul>",
        "slug": "9-benagil",
        "total_activities": 26,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/49-shrine-s320181207-4-1ht8xu0-1544176246.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/49-shrine-s320181207-4-1ht8xu0-1544176246.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/49-shrine-s320181207-4-1ht8xu0-1544176246.jpg"
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
              "id": "107",
              "type": "activity"
            },
            {
              "id": "106",
              "type": "activity"
            },
            {
              "id": "3",
              "type": "activity"
            },
            {
              "id": "480",
              "type": "activity"
            },
            {
              "id": "105",
              "type": "activity"
            },
            {
              "id": "2",
              "type": "activity"
            },
            {
              "id": "4",
              "type": "activity"
            },
            {
              "id": "482",
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
              "id": "62",
              "type": "activity"
            },
            {
              "id": "61",
              "type": "activity"
            },
            {
              "id": "51",
              "type": "activity"
            },
            {
              "id": "100",
              "type": "activity"
            },
            {
              "id": "463",
              "type": "activity"
            },
            {
              "id": "347",
              "type": "activity"
            },
            {
              "id": "601",
              "type": "activity"
            },
            {
              "id": "60",
              "type": "activity"
            },
            {
              "id": "466",
              "type": "activity"
            },
            {
              "id": "102",
              "type": "activity"
            },
            {
              "id": "346",
              "type": "activity"
            },
            {
              "id": "464",
              "type": "activity"
            },
            {
              "id": "456",
              "type": "activity"
            },
            {
              "id": "14",
              "type": "activity"
            },
            {
              "id": "16",
              "type": "activity"
            },
            {
              "id": "440",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "7",
      "type": "destination",
      "attributes": {
        "id": 7,
        "name": "Azores",
        "short_description": "In the middle of the Atlantic Ocean, between Europe and America, lie the Portuguese islands of the Azores.",
        "description": "<div>In the middle of the Atlantic Ocean, between Europe and America, lie the Portuguese islands of the Azores. Untouched nature, breathtaking views, volcanic lakes and hot springs await you in this magical place.&nbsp;<\/div><div>There\u2019s no better way to discover the islands than on one of the boat tours in Azores! There are many types of boat tours in Azores, like fishing, dolphin watching and even whale watching! And once you get back on solid ground after a boat tour in Azores, you have the rest of the island to discover. Go for an adventurous hike in the green mountains or taste some local seafood. Outdoor-lovers and active people will have the best time here, and if you go on a boat tour in Azores you have the seemingly infinite space of the Atlantic Ocean to discover!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia das Mil\u00edcias - S\u00e3o Miguel<\/li><li>Our favorite restaurant: Rotas da Ilha Verde - S\u00e3o Miguel<\/li><li>Our favorite boat tour in Azores: Swimming with dolphins in S\u00e3o Miguel<\/li><\/ul>",
        "slug": "7-azores",
        "total_activities": 14,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/47-shrine20181211-97273-64579u-1544546422.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/47-shrine20181211-97273-64579u-1544546422.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/47-shrine20181211-97273-64579u-1544546422.jpg"
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
              "id": "389",
              "type": "activity"
            },
            {
              "id": "387",
              "type": "activity"
            },
            {
              "id": "390",
              "type": "activity"
            },
            {
              "id": "388",
              "type": "activity"
            },
            {
              "id": "116",
              "type": "activity"
            },
            {
              "id": "114",
              "type": "activity"
            },
            {
              "id": "115",
              "type": "activity"
            },
            {
              "id": "223",
              "type": "activity"
            },
            {
              "id": "224",
              "type": "activity"
            },
            {
              "id": "222",
              "type": "activity"
            },
            {
              "id": "221",
              "type": "activity"
            },
            {
              "id": "441",
              "type": "activity"
            },
            {
              "id": "439",
              "type": "activity"
            },
            {
              "id": "378",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "12",
      "type": "destination",
      "attributes": {
        "id": 12,
        "name": "Cascais",
        "short_description": "Once a quiet fishertown, Cascais has developed into a hip little town just outside of Lisbon. ",
        "description": "<div>Once a quiet fishertown, Cascais has developed into a hip little town just outside of Lisbon. Now famous for delicious restaurants and a nice center with shops for people with good taste, people from all over the world come to Cascais to stroll along with the locals.<\/div><div>Around Cascais you have a lot of beautiful beaches to choose from to enjoy the sun. Praia do Guincho is the best one for fans of surfing. Surfing in Cascais is one of the top things to do, as well as going for a SUP tour or learn kitesurfing. A SUP tour in Cascais is a fun way to spend your holidays, and there\u2019s even the possibility for SUP yoga!&nbsp;<\/div><div>Cascais is the perfect day trip destination if you are staying in Lisbon, or those who want to be close to a city but still enjoy less crowded beaches with a more typical portuguese village flair.<\/div><div><br><\/div><ul><li>Our favorite beach: Praia do Guincho<\/li><li>Our favorite restaurant: Fortaleza do Guincho<\/li><li>Our favorite water sport in Cascais: Paddle yoga in Cascais<\/li><\/ul>",
        "slug": "12-cascais",
        "total_activities": 16,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/52-shrine20181211-97273-1l56o94-1544546553.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/52-shrine20181211-97273-1l56o94-1544546553.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/52-shrine20181211-97273-1l56o94-1544546553.jpg"
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
              "id": "393",
              "type": "activity"
            },
            {
              "id": "131",
              "type": "activity"
            },
            {
              "id": "132",
              "type": "activity"
            },
            {
              "id": "379",
              "type": "activity"
            },
            {
              "id": "565",
              "type": "activity"
            },
            {
              "id": "474",
              "type": "activity"
            },
            {
              "id": "473",
              "type": "activity"
            },
            {
              "id": "469",
              "type": "activity"
            },
            {
              "id": "475",
              "type": "activity"
            },
            {
              "id": "471",
              "type": "activity"
            },
            {
              "id": "470",
              "type": "activity"
            },
            {
              "id": "406",
              "type": "activity"
            },
            {
              "id": "454",
              "type": "activity"
            },
            {
              "id": "380",
              "type": "activity"
            },
            {
              "id": "533",
              "type": "activity"
            },
            {
              "id": "130",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "19",
      "type": "destination",
      "attributes": {
        "id": 19,
        "name": "Lisbon",
        "short_description": "Being one of the oldest cities in the world, the Portuguese capital city is one of the top destinations for city trips, thanks to its location right by the Atlantic Ocean and its multicultural and metropolitan flair. ",
        "description": "<div>Being one of the oldest cities in the world, the Portuguese capital city is one of the top destinations for city trips, thanks to its location right by the Atlantic Ocean and its multicultural and metropolitan flair.&nbsp;<\/div><div>There\u2019s a lot to discover in this vibrant city, from a busy and unique nightlife in \u201cBairro Alto\u201d over architectural jewels spread all over town to beautiful beaches just outside of the cosmopolitan capital.&nbsp;<\/div><div>Boat tours in Lisbon are especially popular to discover the most important spots. You can choose from relaxing sailing tours or go on a wild boat party in Lisbon. Whatever boat tour in Lisbon you choose to do, we guarantee you a great experience and the most fun way to discover the main landmarks of the capital without getting too hot. Because with 290 sunny days on average, you have to be very unlucky to visit Lisbon on a cloudy day!<\/div><div><br><\/div><ul><li>Our favorite beach: Costa da Caparica<\/li><li>Our favorite restaurant: Ponto Final - Cacilhas<\/li><li>Our favorite boat tour in Lisbon: Sunset tour on a vintage boat in Lisbon<\/li><li>Our favorite water sport in Lisbon: Coasteering in Sesimbra<\/li><\/ul>",
        "slug": "19-lisbon",
        "total_activities": 69,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/59-shrine-s320181207-4-1emyx0c-1544177235.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/59-shrine-s320181207-4-1emyx0c-1544177235.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/59-shrine-s320181207-4-1emyx0c-1544177235.jpg"
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
              "id": "380",
              "type": "activity"
            },
            {
              "id": "54",
              "type": "activity"
            },
            {
              "id": "382",
              "type": "activity"
            },
            {
              "id": "386",
              "type": "activity"
            },
            {
              "id": "97",
              "type": "activity"
            },
            {
              "id": "118",
              "type": "activity"
            },
            {
              "id": "121",
              "type": "activity"
            },
            {
              "id": "122",
              "type": "activity"
            },
            {
              "id": "123",
              "type": "activity"
            },
            {
              "id": "131",
              "type": "activity"
            },
            {
              "id": "132",
              "type": "activity"
            },
            {
              "id": "141",
              "type": "activity"
            },
            {
              "id": "204",
              "type": "activity"
            },
            {
              "id": "207",
              "type": "activity"
            },
            {
              "id": "130",
              "type": "activity"
            },
            {
              "id": "473",
              "type": "activity"
            },
            {
              "id": "201",
              "type": "activity"
            },
            {
              "id": "503",
              "type": "activity"
            },
            {
              "id": "475",
              "type": "activity"
            },
            {
              "id": "313",
              "type": "activity"
            },
            {
              "id": "527",
              "type": "activity"
            },
            {
              "id": "361",
              "type": "activity"
            },
            {
              "id": "471",
              "type": "activity"
            },
            {
              "id": "469",
              "type": "activity"
            },
            {
              "id": "500",
              "type": "activity"
            },
            {
              "id": "455",
              "type": "activity"
            },
            {
              "id": "515",
              "type": "activity"
            },
            {
              "id": "445",
              "type": "activity"
            },
            {
              "id": "510",
              "type": "activity"
            },
            {
              "id": "385",
              "type": "activity"
            },
            {
              "id": "476",
              "type": "activity"
            },
            {
              "id": "453",
              "type": "activity"
            },
            {
              "id": "470",
              "type": "activity"
            },
            {
              "id": "497",
              "type": "activity"
            },
            {
              "id": "206",
              "type": "activity"
            },
            {
              "id": "381",
              "type": "activity"
            },
            {
              "id": "474",
              "type": "activity"
            },
            {
              "id": "401",
              "type": "activity"
            },
            {
              "id": "533",
              "type": "activity"
            },
            {
              "id": "575",
              "type": "activity"
            },
            {
              "id": "576",
              "type": "activity"
            },
            {
              "id": "448",
              "type": "activity"
            },
            {
              "id": "383",
              "type": "activity"
            },
            {
              "id": "498",
              "type": "activity"
            },
            {
              "id": "454",
              "type": "activity"
            },
            {
              "id": "119",
              "type": "activity"
            },
            {
              "id": "166",
              "type": "activity"
            },
            {
              "id": "452",
              "type": "activity"
            },
            {
              "id": "579",
              "type": "activity"
            },
            {
              "id": "165",
              "type": "activity"
            },
            {
              "id": "356",
              "type": "activity"
            },
            {
              "id": "239",
              "type": "activity"
            },
            {
              "id": "379",
              "type": "activity"
            },
            {
              "id": "393",
              "type": "activity"
            },
            {
              "id": "240",
              "type": "activity"
            },
            {
              "id": "98",
              "type": "activity"
            },
            {
              "id": "391",
              "type": "activity"
            },
            {
              "id": "120",
              "type": "activity"
            },
            {
              "id": "237",
              "type": "activity"
            },
            {
              "id": "241",
              "type": "activity"
            },
            {
              "id": "317",
              "type": "activity"
            },
            {
              "id": "400",
              "type": "activity"
            },
            {
              "id": "402",
              "type": "activity"
            },
            {
              "id": "406",
              "type": "activity"
            },
            {
              "id": "499",
              "type": "activity"
            },
            {
              "id": "501",
              "type": "activity"
            },
            {
              "id": "509",
              "type": "activity"
            },
            {
              "id": "565",
              "type": "activity"
            },
            {
              "id": "595",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "20",
      "type": "destination",
      "attributes": {
        "id": 20,
        "name": "Madeira",
        "short_description": "On the volcanic island of Madeira, about 700 km west from Lisbon, you can find one of the 7 Wonder Beaches of Portugal, the beach of Porto Santo. But this small group of islands has a lot more to offer than this golden sand beach! ",
        "description": "<div>On the volcanic island of Madeira, about 700 km west from Lisbon, you can find one of the 7 Wonder Beaches of Portugal, the beach of Porto Santo. But this small group of islands has a lot more to offer than this golden sand beach!&nbsp;<\/div><div>Hikers can explore the trails along the famous \u201clevadas\u201d, small irrigation canals that you can follow from the North until the South of the island and that will show you every corner of this magical place. If you wish to enjoy the sea, hop aboard on one of the plenty dolphin watching boat tours in Madeira.&nbsp; For a once in a lifetime experience, swimming with dolphins in Madeira is our recommendation. The warm water around the island also invites for a surf lesson in Madeira, or any other of the plenty water sport activities you can do here.&nbsp;<\/div><div>Madeira is one of our secret highlights for boat tours and dolphin watching tours in Portugal, taking you on an adventure in the middle of the Atlantic Ocean!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia da Prainha \u2013 Cani\u00e7al<\/li><li>Our favorite restaurant: Papa Manuel do Lido<\/li><li>Our favorite boat tour in Madeira: Swimming with dolphins in Madeira<\/li><li>Our favorite water sport in Madeira: Surf in Madeira<\/li><\/ul>",
        "slug": "20-madeira",
        "total_activities": 26,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/60-shrine-s320181207-4-mktgms-1544177339.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/60-shrine-s320181207-4-mktgms-1544177339.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/60-shrine-s320181207-4-mktgms-1544177339.jpg"
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
              "id": "384",
              "type": "activity"
            },
            {
              "id": "327",
              "type": "activity"
            },
            {
              "id": "205",
              "type": "activity"
            },
            {
              "id": "318",
              "type": "activity"
            },
            {
              "id": "320",
              "type": "activity"
            },
            {
              "id": "169",
              "type": "activity"
            },
            {
              "id": "319",
              "type": "activity"
            },
            {
              "id": "329",
              "type": "activity"
            },
            {
              "id": "328",
              "type": "activity"
            },
            {
              "id": "326",
              "type": "activity"
            },
            {
              "id": "56",
              "type": "activity"
            },
            {
              "id": "143",
              "type": "activity"
            },
            {
              "id": "177",
              "type": "activity"
            },
            {
              "id": "55",
              "type": "activity"
            },
            {
              "id": "526",
              "type": "activity"
            },
            {
              "id": "397",
              "type": "activity"
            },
            {
              "id": "523",
              "type": "activity"
            },
            {
              "id": "524",
              "type": "activity"
            },
            {
              "id": "396",
              "type": "activity"
            },
            {
              "id": "525",
              "type": "activity"
            },
            {
              "id": "522",
              "type": "activity"
            },
            {
              "id": "220",
              "type": "activity"
            },
            {
              "id": "210",
              "type": "activity"
            },
            {
              "id": "209",
              "type": "activity"
            },
            {
              "id": "218",
              "type": "activity"
            },
            {
              "id": "219",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "15",
      "type": "destination",
      "attributes": {
        "id": 15,
        "name": "Faro",
        "short_description": "Faro has a lot more to offer than just an Airport where most travelers land when they come to the Algarve.",
        "description": "<div>Faro has a lot more to offer than just an Airport where most travelers land when they come to the Algarve. Its beautiful marina and the cute little old part of town offer a charming Portuguese flair and loads of caf\u00e9s and restaurants.<\/div><div>Oceanwise, there\u2019s a lot to discover! You can go on a boat tour in Faro to go dolphin watching or on a boat tour in Ria Formosa, a beautiful Nature Reserve with a unique flora and fauna. On a boat tour in Ria Formosa you will be able to spot a lot of special species, which is why boat tours in Ria Formosa are especially popular amongst bird watchers and nature lovers. &nbsp;<\/div><div>Fishing in Faro is also very popular, just like kayaking in Ria Formosa. People who are looking for sea activities on their holidays will have loads to do in Faro!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia do Farol<\/li><li>Our favorite restaurant: A Venda<\/li><li>Our favorite boat tour in Faro: Solar boat tour in Ria Formosa<\/li><li>Our favorite water sport in Faro: Half day kayaking in Ria Formosa<\/li><\/ul>",
        "slug": "15-faro",
        "total_activities": 13,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/55-shrine-s320181207-4-jggwmt-1544176956.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/55-shrine-s320181207-4-jggwmt-1544176956.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/55-shrine-s320181207-4-jggwmt-1544176956.jpg"
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
              "id": "608",
              "type": "activity"
            },
            {
              "id": "168",
              "type": "activity"
            },
            {
              "id": "191",
              "type": "activity"
            },
            {
              "id": "214",
              "type": "activity"
            },
            {
              "id": "200",
              "type": "activity"
            },
            {
              "id": "194",
              "type": "activity"
            },
            {
              "id": "375",
              "type": "activity"
            },
            {
              "id": "215",
              "type": "activity"
            },
            {
              "id": "193",
              "type": "activity"
            },
            {
              "id": "192",
              "type": "activity"
            },
            {
              "id": "213",
              "type": "activity"
            },
            {
              "id": "374",
              "type": "activity"
            },
            {
              "id": "373",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "27",
      "type": "destination",
      "attributes": {
        "id": 27,
        "name": "Sagres",
        "short_description": "Sagres is a very unique place along the Southern Coast of Portugal.",
        "description": "<div>Sagres is a very unique place along the Southern Coast of Portugal. Once believed to be the end of the world, the landscape and overall feeling of this little beach town is this of nature in its purest element.&nbsp;<\/div><div>The wildness of Sagres has made this little town especially popular amongst travelers who seek a place not as touristy as the other coastal towns of the Algarve. Due to its beaches that are open to various different directions, it has become one of the main spots for surfing in the Algarve.<\/div><div>Surfing in Sagres is perfect for all levels, and there are plenty of surf schools to choose from. There are also a lot of other things to do in Sagres: kayaking and SUP for example, or going on a boat tour in Sagres and be amazed by the unique coastline of the most Western point of the Algarve!<\/div><div><br><\/div><ul><li>Our favorite beach: Martinhal Beach<\/li><li>Our favorite restaurant: Three Little Birds<\/li><li>Our favorite boat tour in Sagres: Dolphin Watching in Sagres<\/li><li>Our favorite water sport in Sagres: Learn Surfing in Sagres<\/li><\/ul>",
        "slug": "27-sagres",
        "total_activities": 9,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/67-shrine-s320181207-4-15bhmkw-1544178243.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/67-shrine-s320181207-4-15bhmkw-1544178243.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/67-shrine-s320181207-4-15bhmkw-1544178243.jpg"
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
              "id": "129",
              "type": "activity"
            },
            {
              "id": "150",
              "type": "activity"
            },
            {
              "id": "126",
              "type": "activity"
            },
            {
              "id": "472",
              "type": "activity"
            },
            {
              "id": "151",
              "type": "activity"
            },
            {
              "id": "211",
              "type": "activity"
            },
            {
              "id": "127",
              "type": "activity"
            },
            {
              "id": "149",
              "type": "activity"
            },
            {
              "id": "128",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "22",
      "type": "destination",
      "attributes": {
        "id": 22,
        "name": "Olh\u00e3o",
        "short_description": "Situated in the Eastern Algarve, this Portuguese town is especially famous for its seafood and the fishermen\u2019s port! If you love some fresh fish, you will be in heaven here! From Olh\u00e3o, you can go on beautiful boat tours in Ria Formosa, a Nature Reserve with unique flora and fauna! If you go on a boat tour in Ria Formosa, you will surely see some birds and fish you won\u2019t find anywhere else!",
        "description": "<div>Situated in the Eastern Algarve, this Portuguese town is especially famous for its seafood and the fishermen\u2019s port! If you love some fresh fish, you will be in heaven here! From Olh\u00e3o, you can go on beautiful boat tours in Ria Formosa, a Nature Reserve with unique flora and fauna! If you go on a boat tour in Ria Formosa, you will surely see some birds and fish you won\u2019t find anywhere else!<\/div><div>Olh\u00e3o doesn\u2019t have any beaches right off the coast, but there are beautiful little islands around the town, so be sure to go on a boat tour in Olh\u00e3o to explore some of them, like Ilha do Farol or Ilha da Armona. Or get on one of the dolphin watching tours to see these beautiful creatures in their natural habitat!&nbsp;<\/div><div>The little town is perfect for a dinner night out as the Moorish influences makes the scenery unique and incomparable to any other town in the Algarve!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia da Fuseta<\/li><li>Our favorite restaurant: Bioco Olh\u00e3o<\/li><li>Our favorite boat tour in Olh\u00e3o: Full day private sailing in Olh\u00e3o<\/li><li>Our favorite water sport in Olh\u00e3o: Seahorse observation in Ria Formosa<\/li><\/ul>",
        "slug": "22-olhao",
        "total_activities": 11,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/62-shrine-s320181207-4-16wv3hb-1544177500.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/62-shrine-s320181207-4-16wv3hb-1544177500.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/62-shrine-s320181207-4-16wv3hb-1544177500.jpg"
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
              "id": "153",
              "type": "activity"
            },
            {
              "id": "152",
              "type": "activity"
            },
            {
              "id": "605",
              "type": "activity"
            },
            {
              "id": "458",
              "type": "activity"
            },
            {
              "id": "612",
              "type": "activity"
            },
            {
              "id": "604",
              "type": "activity"
            },
            {
              "id": "154",
              "type": "activity"
            },
            {
              "id": "451",
              "type": "activity"
            },
            {
              "id": "216",
              "type": "activity"
            },
            {
              "id": "617",
              "type": "activity"
            },
            {
              "id": "156",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "23",
      "type": "destination",
      "attributes": {
        "id": 23,
        "name": "Portim\u00e3o",
        "short_description": "The biggest city in the Western Algarve is perfect for all those who love being by the Ocean but also enjoy an afternoon spent doing some shopping and strolling along a promenade with a vibrant life! ",
        "description": "<div>The biggest city in the Western Algarve is perfect for all those who love being by the Ocean but also enjoy an afternoon spent doing some shopping and strolling along a promenade with a vibrant life! In Portim\u00e3o, you have the best of both worlds. You\u2019ll find plenty of beautiful beaches to choose from for sunbathing and loads of ocean-related activities to do.&nbsp;<\/div><div>You can go on a boat tour in Portim\u00e3o and head over to the famous Benagil caves, go on a dolphin watching tour or just relax on a chilled sunset tour along the beautiful coast of the Algarve. For the ones who prefer to stay on land, just relax at Praia da Rocha or Praia Jo\u00e3o de Arens!<\/div><div>If you wish to enjoy some seafood, there are enough seafood restaurants to choose from in the Marina of Portim\u00e3o or the old town!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia Jo\u00e3o de Arens<\/li><li>Our favorite restaurant: Taberna da Mar\u00e9<\/li><li>Our favorite boat tour in Portim\u00e3o: Motorboat rental in Portim\u00e3o<\/li><li>Our favorite water sport in Portim\u00e3o: Kayak in Portim\u00e3o<\/li><\/ul>",
        "slug": "23-portimao",
        "total_activities": 38,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/63-shrine-s320181207-4-1940mi-1544177582.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/63-shrine-s320181207-4-1940mi-1544177582.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/63-shrine-s320181207-4-1940mi-1544177582.jpg"
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
              "id": "103",
              "type": "activity"
            },
            {
              "id": "108",
              "type": "activity"
            },
            {
              "id": "332",
              "type": "activity"
            },
            {
              "id": "109",
              "type": "activity"
            },
            {
              "id": "110",
              "type": "activity"
            },
            {
              "id": "111",
              "type": "activity"
            },
            {
              "id": "113",
              "type": "activity"
            },
            {
              "id": "347",
              "type": "activity"
            },
            {
              "id": "53",
              "type": "activity"
            },
            {
              "id": "145",
              "type": "activity"
            },
            {
              "id": "352",
              "type": "activity"
            },
            {
              "id": "187",
              "type": "activity"
            },
            {
              "id": "188",
              "type": "activity"
            },
            {
              "id": "189",
              "type": "activity"
            },
            {
              "id": "456",
              "type": "activity"
            },
            {
              "id": "370",
              "type": "activity"
            },
            {
              "id": "457",
              "type": "activity"
            },
            {
              "id": "369",
              "type": "activity"
            },
            {
              "id": "601",
              "type": "activity"
            },
            {
              "id": "353",
              "type": "activity"
            },
            {
              "id": "331",
              "type": "activity"
            },
            {
              "id": "394",
              "type": "activity"
            },
            {
              "id": "112",
              "type": "activity"
            },
            {
              "id": "60",
              "type": "activity"
            },
            {
              "id": "368",
              "type": "activity"
            },
            {
              "id": "371",
              "type": "activity"
            },
            {
              "id": "464",
              "type": "activity"
            },
            {
              "id": "372",
              "type": "activity"
            },
            {
              "id": "102",
              "type": "activity"
            },
            {
              "id": "346",
              "type": "activity"
            },
            {
              "id": "466",
              "type": "activity"
            },
            {
              "id": "324",
              "type": "activity"
            },
            {
              "id": "330",
              "type": "activity"
            },
            {
              "id": "355",
              "type": "activity"
            },
            {
              "id": "399",
              "type": "activity"
            },
            {
              "id": "440",
              "type": "activity"
            },
            {
              "id": "481",
              "type": "activity"
            },
            {
              "id": "482",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "24",
      "type": "destination",
      "attributes": {
        "id": 24,
        "name": "Peniche",
        "short_description": "Peniche is probably most famous nowadays for Supertubos, the world-class surfspot that is also a stop at the WSL Tour, bringing the world\u2019s best surfers to this little town every autumn! ",
        "description": "<div>Peniche is probably most famous nowadays for Supertubos, the world-class surfspot that is also a stop at the WSL Tour, bringing the world\u2019s best surfers to this little town every autumn! Therefore it\u2019s no secret anymore, that the waves in Peniche and in the neighbour village Baleal are among the best in Portugal! This attracts thousands of surfers every year to this little peninsula, just about 1-hour drive away from Lisbon!<\/div><div>However, you can also spend some great time off from surfing wandering through the historic town of Peniche. The fortress of Peniche is very impressive! And of course you should visit the natural reserve Ilhas Berlengas! This group of islands remains almost completely untouched, and is home to a big variety of seabirds and other impressive flora and fauna! So Peniche is a great spot to spend your holidays or to go for a day trip if you\u2019re staying in Lisbon. And if you like surfing, you\u2019ll love the surfer vibe and waves in and around Peniche!<\/div><div><br><\/div><ul><li>Our favorite beach: Baleal Beach<\/li><li>Our favorite restaurant: Cantina de Ferrel<\/li><li>Our favorite boat tour in Peniche: Boat tour to Berlenga Islands<\/li><li>Our favorite water sport in Peniche: Half day fishing in Peniche<\/li><\/ul>",
        "slug": "24-peniche",
        "total_activities": 3,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/64-shrine-s320181207-4-18xe2ci-1544177645.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/64-shrine-s320181207-4-18xe2ci-1544177645.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/64-shrine-s320181207-4-18xe2ci-1544177645.jpg"
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
              "id": "598",
              "type": "activity"
            },
            {
              "id": "573",
              "type": "activity"
            },
            {
              "id": "572",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "25",
      "type": "destination",
      "attributes": {
        "id": 25,
        "name": "Oporto",
        "short_description": "There\u2019s plenty of reasons why Ooorto has become one of the most popular destinations for travelers who like to visit cities! ",
        "description": "<div>There\u2019s plenty of reasons why Oporto has become one of the most popular destinations for travelers who like to visit cities! The seven bridges across the Douro River, the famous Port Wine Cellars, beautiful city beaches like Foz do Douro and Matosinhos Beach are just some of those reasons!<\/div><div>The view you have over the old part of the city when standing on the most popular bridge, Ponte de Dom Luis I, is unique and breathtaking! Gastronomy is booming in Oporto, as well as Art and Modern Culture. Culturally interested travelers must visit Serralves Museum and Casa da M\u00fasica.<\/div><div>Oporto\u2019s waterfront location also means there are a lot of ocean activities to do! Surfing in Oporto is possible all year round and you can go straight to a hip caf\u00e9 after surfing in Matosinhos Beach! It\u2019s the perfect destination for city lovers who also want to feel the kick of surfing in Oporto!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia dos Ingleses<\/li><li>Our favorite restaurant: Taberninha Do Manel - Vila Nova de Gaia<\/li><li>Our favorite water sport in Porto: Matosinhos Surf Lesson<\/li><\/ul><div><br><br><\/div>",
        "slug": "25-oporto",
        "total_activities": 7,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/65-shrine-s320181207-4-1vhd7v0-1544178093.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/65-shrine-s320181207-4-1vhd7v0-1544178093.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/65-shrine-s320181207-4-1vhd7v0-1544178093.jpg"
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
              "id": "225",
              "type": "activity"
            },
            {
              "id": "227",
              "type": "activity"
            },
            {
              "id": "226",
              "type": "activity"
            },
            {
              "id": "228",
              "type": "activity"
            },
            {
              "id": "231",
              "type": "activity"
            },
            {
              "id": "229",
              "type": "activity"
            },
            {
              "id": "230",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "28",
      "type": "destination",
      "attributes": {
        "id": 28,
        "name": "Sesimbra",
        "short_description": "Sesimbra is becoming more and more popular among travelers from all over the world. ",
        "description": "<div>Sesimbra is becoming more and more popular among travelers from all over the world. With its long-stretched sandy beaches and the proximity to the beautiful Serra da Arr\u00e1bida natural park, visitors have a lot to choose from! You can visit Sesimbra on a day trip from Lisbon, which is only 40 minutes away.<\/div><div>Diving in Sesimbra is one of the top things to do, and it\u2019s one of the best spots in all of Portugal for diving and snorkeling. If you decide to go scuba diving in Sesimbra, be ready to explore an amazing underwater world with caves, wrecks and beautiful reefs all around you.<\/div><div>If you rather stay above sea level, you can embark on one of the fun boat tours in Sesimbra, go dolphin watching or even fishing in Sesimbra. After the fresh sea breeze, you\u2019ll be happy to know that Sesimbra is a true seafood paradise!<\/div><div><br><\/div><ul><li>Our favorite beach: Ribeira do Cavalo Beach<\/li><li>Our favorite restaurant: Praia Mar<\/li><li>Our favorite boat tour in Sesimbra: Fishing in Sesimbra<\/li><li>Our favorite water sport in: Scuba Diving in Sesimbra<\/li><\/ul>",
        "slug": "28-sesimbra",
        "total_activities": 12,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/68-shrine-s320181207-4-mprrbh-1544178321.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/68-shrine-s320181207-4-mprrbh-1544178321.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/68-shrine-s320181207-4-mprrbh-1544178321.jpg"
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
              "id": "401",
              "type": "activity"
            },
            {
              "id": "402",
              "type": "activity"
            },
            {
              "id": "400",
              "type": "activity"
            },
            {
              "id": "98",
              "type": "activity"
            },
            {
              "id": "122",
              "type": "activity"
            },
            {
              "id": "97",
              "type": "activity"
            },
            {
              "id": "121",
              "type": "activity"
            },
            {
              "id": "201",
              "type": "activity"
            },
            {
              "id": "120",
              "type": "activity"
            },
            {
              "id": "500",
              "type": "activity"
            },
            {
              "id": "119",
              "type": "activity"
            },
            {
              "id": "118",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "31",
      "type": "destination",
      "attributes": {
        "id": 31,
        "name": "Tavira",
        "short_description": "If you want to immerse yourself in Southern Portuguese culture without the touristic crowd of the central Algarve, Tavira is the place for you to spend your holidays at.",
        "description": "<div>If you want to immerse yourself in Southern Portuguese culture without the touristic crowd of the central Algarve, Tavira is the place for you to spend your holidays at. This little town in the Eastern Algarve has maintained its authentic Portuguese charme and the family-run businesses will give you a glimpse of what Portugal is all about.<\/div><div>The proximity to the Natural Park of Ria Formosa invites for a boat tour in Tavira to discover the local flora and fauna of that beautiful park. Just outside of the town, you can visit the island <em>Ilha de Tavira<\/em> and relax on one of the sandy beaches or go on fishing in Tavira. Fishing in Tavira are very popular and promises the biggest catch of your life! You can choose to go Big Game Fishing in Tavira or even opt for Shark Fishing in Tavira and feel the adrenaline rushing through your veins!<\/div><div><br><\/div><ul><li>Our favorite beach: Cacela Velha<\/li><li>Our favorite restaurant: Restaurante O Castelo<\/li><li>Our favorite boat tour in Tavira: Sunset Tour in Tavira<\/li><li>Our favorite water sport in Tavira: Big Game Fishing in Tavira<\/li><\/ul>",
        "slug": "31-tavira",
        "total_activities": 8,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/71-shrine-s320181207-4-1huab5o-1544178585.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/71-shrine-s320181207-4-1huab5o-1544178585.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/71-shrine-s320181207-4-1huab5o-1544178585.jpg"
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
              "id": "47",
              "type": "activity"
            },
            {
              "id": "43",
              "type": "activity"
            },
            {
              "id": "69",
              "type": "activity"
            },
            {
              "id": "44",
              "type": "activity"
            },
            {
              "id": "48",
              "type": "activity"
            },
            {
              "id": "46",
              "type": "activity"
            },
            {
              "id": "146",
              "type": "activity"
            },
            {
              "id": "45",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "34",
      "type": "destination",
      "attributes": {
        "id": 34,
        "name": "Vilamoura",
        "short_description": "Travelers seeking a rather exclusive resort in the central Algarve will be pleased to find exquisite taste and a touch of luxury in the town of Vilamoura. ",
        "description": "<div>Travelers seeking a rather exclusive resort in the central Algarve will be pleased to find exquisite taste and a touch of luxury in the town of Vilamoura. Golfers have probably heard this name before, since Vilamoura is one of the most beautiful spots for a golfing holiday.<\/div><div>The beaches are clean and the ocean is calm, inviting the whole family for a relaxing and refreshing dip. The Marina is the heart of this town, which is also why there are plenty of boat tours in Vilamoura to choose from.<\/div><div>Head aboard of one of the sailing boat tours in Vilamoura or go for a BBQ tour on the ocean. If you are looking for some sport fishing, Shark fishing, Big Game fishing, or reef fishing in Vilamoura promise to be a great experience on your holiday in the Algarve. The calm waters are also perfect for a SUP Tour in Vilamoura. Or hop on board of one of the Grotto Tours to discover the famous Benagil Caves. The choice is yours!<\/div><div><br><\/div><ul><li>Our favorite beach: Praia da Fal\u00e9sia<\/li><li>Our favorite restaurant: Chilly Lounge<\/li><li>Our favorite boat tour in Vilamoura: BBQ cruise in Vilamoura during sunset<\/li><li>Our favorite water sport in Vilamoura: Jet Ski rental in Vilamoura<\/li><\/ul>",
        "slug": "34-vilamoura",
        "total_activities": 39,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/74-shrine-s320181207-4-9w343i-1544178779.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/74-shrine-s320181207-4-9w343i-1544178779.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/74-shrine-s320181207-4-9w343i-1544178779.jpg"
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
              "id": "12",
              "type": "activity"
            },
            {
              "id": "13",
              "type": "activity"
            },
            {
              "id": "15",
              "type": "activity"
            },
            {
              "id": "16",
              "type": "activity"
            },
            {
              "id": "17",
              "type": "activity"
            },
            {
              "id": "18",
              "type": "activity"
            },
            {
              "id": "19",
              "type": "activity"
            },
            {
              "id": "20",
              "type": "activity"
            },
            {
              "id": "21",
              "type": "activity"
            },
            {
              "id": "23",
              "type": "activity"
            },
            {
              "id": "24",
              "type": "activity"
            },
            {
              "id": "25",
              "type": "activity"
            },
            {
              "id": "26",
              "type": "activity"
            },
            {
              "id": "29",
              "type": "activity"
            },
            {
              "id": "31",
              "type": "activity"
            },
            {
              "id": "34",
              "type": "activity"
            },
            {
              "id": "35",
              "type": "activity"
            },
            {
              "id": "36",
              "type": "activity"
            },
            {
              "id": "37",
              "type": "activity"
            },
            {
              "id": "38",
              "type": "activity"
            },
            {
              "id": "39",
              "type": "activity"
            },
            {
              "id": "172",
              "type": "activity"
            },
            {
              "id": "447",
              "type": "activity"
            },
            {
              "id": "22",
              "type": "activity"
            },
            {
              "id": "403",
              "type": "activity"
            },
            {
              "id": "33",
              "type": "activity"
            },
            {
              "id": "405",
              "type": "activity"
            },
            {
              "id": "468",
              "type": "activity"
            },
            {
              "id": "404",
              "type": "activity"
            },
            {
              "id": "28",
              "type": "activity"
            },
            {
              "id": "248",
              "type": "activity"
            },
            {
              "id": "173",
              "type": "activity"
            },
            {
              "id": "14",
              "type": "activity"
            },
            {
              "id": "171",
              "type": "activity"
            },
            {
              "id": "117",
              "type": "activity"
            },
            {
              "id": "398",
              "type": "activity"
            },
            {
              "id": "30",
              "type": "activity"
            },
            {
              "id": "27",
              "type": "activity"
            },
            {
              "id": "478",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "1",
      "type": "destination",
      "attributes": {
        "id": 1,
        "name": "Albufeira",
        "short_description": "Albufeira is known as one of the best resorts in Southern Portugal.",
        "description": "<div>Albufeira is known as one of the best resorts in Southern Portugal. In fact, this coastal city has fantastic beaches, beautiful turquoise waters and a unique rocky coastline that makes the Algarve so special. Therefore, boat tours in Albufeira are very popular.<\/div><div>This former fishing village has become a major holiday destination for the ones who look for the best boat tours and watersports in the Algarve and also for a busy nightlife.&nbsp;<\/div><div>Albufeira has a modern marina, where you can find some of the best sea experiences in the Algarve like diving, dolphin watching and other boat trips. Boat tours in Albufeira run all year round. The Marina is surrounded by candy-colored apartments and on its waterfront promenade you can have a nice lunch and drinks.<\/div><div><br><\/div><ul><li>Our favorite beach: Praia de Santa Eul\u00e1lia - Olhos de \u00c1gua<\/li><li>Our favorite restaurant: Vila Joia, Gal\u00e9<\/li><li>Our favorite boat tours in Albufeira: Caves &amp; dolphin watching from Albufeira &nbsp;<\/li><li>Our favorite water sport in Albufeira: First dive Albufeira<\/li><\/ul>",
        "slug": "1-albufeira",
        "total_activities": 29,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/41-shrine-s320181207-4-7cvels-1544175180.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/41-shrine-s320181207-4-7cvels-1544175180.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/41-shrine-s320181207-4-7cvels-1544175180.jpg"
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
              "id": "2",
              "type": "activity"
            },
            {
              "id": "3",
              "type": "activity"
            },
            {
              "id": "4",
              "type": "activity"
            },
            {
              "id": "6",
              "type": "activity"
            },
            {
              "id": "7",
              "type": "activity"
            },
            {
              "id": "8",
              "type": "activity"
            },
            {
              "id": "9",
              "type": "activity"
            },
            {
              "id": "32",
              "type": "activity"
            },
            {
              "id": "57",
              "type": "activity"
            },
            {
              "id": "58",
              "type": "activity"
            },
            {
              "id": "59",
              "type": "activity"
            },
            {
              "id": "104",
              "type": "activity"
            },
            {
              "id": "105",
              "type": "activity"
            },
            {
              "id": "148",
              "type": "activity"
            },
            {
              "id": "167",
              "type": "activity"
            },
            {
              "id": "314",
              "type": "activity"
            },
            {
              "id": "107",
              "type": "activity"
            },
            {
              "id": "5",
              "type": "activity"
            },
            {
              "id": "477",
              "type": "activity"
            },
            {
              "id": "504",
              "type": "activity"
            },
            {
              "id": "217",
              "type": "activity"
            },
            {
              "id": "376",
              "type": "activity"
            },
            {
              "id": "442",
              "type": "activity"
            },
            {
              "id": "106",
              "type": "activity"
            },
            {
              "id": "10",
              "type": "activity"
            },
            {
              "id": "190",
              "type": "activity"
            },
            {
              "id": "479",
              "type": "activity"
            },
            {
              "id": "446",
              "type": "activity"
            },
            {
              "id": "480",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "14",
      "type": "destination",
      "attributes": {
        "id": 14,
        "name": "Dubai",
        "short_description": "Dubai, the city of extremes. If you like it exclusive, extreme and exotic, Dubai is the place to visit! ",
        "description": "<div>Dubai, the city of extremes. If you like it exclusive, extreme and exotic, Dubai is the place to visit! This multicultural city is full of life and you have plenty of things to do in Dubai. You can choose to relax at Jumeirah Beach for example or take a boat tour to explore the most famous tourist attractions like Burj Al Arab, Atlantis Hotel or Palm Jumeirah.&nbsp;<\/div><div>But if you\u2019d like to do something really crazy, you can go skiing in Dubai! Yes you heard right - in the city in the middle of the Arabian desert, where it\u2019s warm and sunny all year around, you can go skiing! And you don\u2019t have to go to a special place for that, just to the Mall! That sums up Dubai life pretty well, we think! Dubai, the city of all possibilities!&nbsp;<\/div><div>And despite the cultural differences, if you respect the local rules, you can enjoy your time here just like in any other big cosmopolitan city!&nbsp;<\/div><div><br><\/div><ul><li>Our favorite beach: Jumeirah Beach&nbsp;<\/li><li>Our favorite restaurant: Little Miss India<\/li><li>Our favorite boat tour in Dubai: Half day boat rental in Dubai<\/li><li>Our favorite water sport in Dubai: Full day fishing charter in Dubai<\/li><\/ul>",
        "slug": "14-dubai",
        "total_activities": 14,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/54-shrine-s320181207-4-16gt61-1544176910.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/54-shrine-s320181207-4-16gt61-1544176910.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/54-shrine-s320181207-4-16gt61-1544176910.jpg"
        },
        "country": {
          "name": "United Arab Emirates",
          "slug": "united-arab-emirates",
          "code": "AE"
        }
      },
      "relationships": {
        "activities": {
          "data": [
            {
              "id": "490",
              "type": "activity"
            },
            {
              "id": "514",
              "type": "activity"
            },
            {
              "id": "486",
              "type": "activity"
            },
            {
              "id": "494",
              "type": "activity"
            },
            {
              "id": "489",
              "type": "activity"
            },
            {
              "id": "487",
              "type": "activity"
            },
            {
              "id": "488",
              "type": "activity"
            },
            {
              "id": "485",
              "type": "activity"
            },
            {
              "id": "495",
              "type": "activity"
            },
            {
              "id": "483",
              "type": "activity"
            },
            {
              "id": "491",
              "type": "activity"
            },
            {
              "id": "484",
              "type": "activity"
            },
            {
              "id": "492",
              "type": "activity"
            },
            {
              "id": "493",
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
    },
    {
      "id": "10",
      "type": "destination",
      "attributes": {
        "id": 10,
        "name": "Benidorm",
        "short_description": "Benidorm, located on the famous Costa Blanca, in close proximity to Alicante, has developed from an all-inclusive holiday destination to a hip and modern city that has a lot to offer for all kinds of travellers.",
        "description": "<div>Benidorm, located on the famous <em>Costa Blanca<\/em>, in close proximity to Alicante, has developed from an all-inclusive holiday destination to a hip and modern city that has a lot to offer for all kinds of travellers. Whether you are looking for a wild and buzzing nightlife, sunbathe all day on one of the two long sandy beaches or want to have an active holiday - in Benidorm you can choose all of it!<\/div><div>With its great location on the warm and calm waters of the Costa Blanca, watersport-lovers will love Benidorm! Did you also know, that on boat tours from Benidorm you have some cute little islands to discover off the coast, like <em>L\u2019illa de Benidorm<\/em>, or Benidorm Island? It\u2019s a great way to escape the crowds for a few hours! And when you get back, head right back into the exciting entertainment offered all around Benidorm - from live concerts, theatre to popular DJs at night, you surely won\u2019t get bored during your stay in Benidorm!&nbsp;<\/div><div><br><\/div><ul><li>Our favorite beach: Playa Levante&nbsp;<\/li><li>Our favorite restaurant: Margem Restobar<\/li><li>Our favorite water sport in Benidorm: Kayak Tour to Benidorm Island<\/li><\/ul>",
        "slug": "10-benidorm",
        "total_activities": 3,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/50-shrine20181211-97273-12p6ysq-1544546445.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/50-shrine20181211-97273-12p6ysq-1544546445.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/50-shrine20181211-97273-12p6ysq-1544546445.jpg"
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
              "id": "613",
              "type": "activity"
            },
            {
              "id": "615",
              "type": "activity"
            },
            {
              "id": "614",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "16",
      "type": "destination",
      "attributes": {
        "id": 16,
        "name": "Gran Canaria",
        "short_description": "Due to the big variety in landscapes, the third largest island of the Canary Islands is also called a miniature continent.",
        "description": "<div>Due to the big variety in landscapes, the third largest island of the Canary Islands is also called a miniature continent. Here you find warm weather pretty much all-year round, inviting you to visit the many attractions the island has to offer!<\/div><div>In the South, you have a buzzing tourist life, with lots of culture, restaurants, bars and of course beautiful beaches where you can simply enjoy the nice sunshine! If you wish to see some more of \u201creal\u201d Gran Canaria, you should definitely also head inlands! The mountains of Gran Canaria are impressive and will amaze you with their natural diversity. From up here you also get a better feeling of the volcanic landscape of Gran Canaria. There are many different trails, for beginners and more advanced hikers. And to freshen up, there are loads of water sport activities offered around the coast!<\/div><div>Gran Canaria is sure to be a great destination for everybody - from active travelers over sunlovers, the island is perfect for all!<\/div><div><br><\/div><ul><li>Our favorite beach: Maspalomas<\/li><li>Our favorite restaurant: Sweet Corner<\/li><li>Our favorite boat tour in Gran Canaria: Whale &amp; dolphin watching in Gran Canaria<\/li><li>Our favorite water sport in Gran Canaria: Snorkeling in Gran Canaria<\/li><\/ul>",
        "slug": "16-gran-canaria",
        "total_activities": 10,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/56-shrine-s320181207-4-10pbejf-1544177004.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/56-shrine-s320181207-4-10pbejf-1544177004.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/56-shrine-s320181207-4-10pbejf-1544177004.jpg"
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
              "id": "571",
              "type": "activity"
            },
            {
              "id": "574",
              "type": "activity"
            },
            {
              "id": "600",
              "type": "activity"
            },
            {
              "id": "530",
              "type": "activity"
            },
            {
              "id": "609",
              "type": "activity"
            },
            {
              "id": "566",
              "type": "activity"
            },
            {
              "id": "513",
              "type": "activity"
            },
            {
              "id": "610",
              "type": "activity"
            },
            {
              "id": "599",
              "type": "activity"
            },
            {
              "id": "516",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "18",
      "type": "destination",
      "attributes": {
        "id": 18,
        "name": "La palma",
        "short_description": "Known as \u201cLa isla bonita\u201d, which means the pretty island, La Palma is surely the jewel of the Canary Islands!",
        "description": "<div>Known as \u201cLa isla bonita\u201d, which means the pretty island, La Palma is surely the jewel of the Canary Islands! Green forests, in which you can hike along waterfalls and explore the distinct flair of a volcanic island, black sanded beaches and one of the world\u2019s best spots for stargazing - all of this makes La Palma a special place to visit.<\/div><div>Boat tours in La Palma will take you to see dolphins and whales for example. And after a boat tour in La Palma you can go on one of the famous hikes across the islands or for a stroll in the charming town of Santa Cruz de La Palma.<\/div><div>A whale watching tour in La Palma is certainly the highlight of the many things to do on this magical island. And on sleepless nights, head up to the observatory and get as close as possible to the mysteries of the universe!<\/div><div><br><\/div><ul><li>Our favorite beach: Playa de Nogales<\/li><li>Our favorite restaurant: Chipi-Chipi<\/li><li>Our favorite boat tour in La Palma: Whale and Dolphin Safari<\/li><\/ul>",
        "slug": "18-la-palma",
        "total_activities": 3,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/58-shrine-s320181207-4-xb08nr-1544177122.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/58-shrine-s320181207-4-xb08nr-1544177122.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/58-shrine-s320181207-4-xb08nr-1544177122.jpg"
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
              "id": "250",
              "type": "activity"
            },
            {
              "id": "252",
              "type": "activity"
            },
            {
              "id": "251",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "17",
      "type": "destination",
      "attributes": {
        "id": 17,
        "name": "Ibiza",
        "short_description": "What comes to your mind when you hear \u201cIbiza\u201d? Most of us probably associate the name of this Balearic island in the Mediterranean with a buzzing nightlife, boho-chic, and a big hippie community!",
        "description": "<div>What comes to your mind when you hear \u201cIbiza\u201d? Most of us probably associate the name of this Balearic island in the Mediterranean with a buzzing nightlife, boho-chic, and a big hippie community! During Summer, most young people travelling to Ibiza do so to enjoy the sun during the day and the unique nightlife once the sun sets!<\/div><div>Actually there is much more to this little island! If you visit Ibiza in Spring or Autumn for example, you will be able to enjoy the amazing nature. Even in Summer there are parts of the island that are rather empty and attract a whole other kind of tourists. Santa Eul\u00e1lia and San Miguel are just some of the pretty places you can visit to enjoy the beautiful beaches and crystalline waters. Ibiza is blessed with such a variation in things to do and see, that it is a great all-year around destination for all kinds of travellers - be it family, spiritual seekers or bachelor parties!<\/div><div><br><\/div><ul><li>Our favorite beach: Cala Salada<\/li><li>Our favorite restaurant: Caos Ibiza<\/li><li>Our favorite boat tour in Ibiza: Private full day boat tour in Ibiza<\/li><li>Our favorite water sport in Ibiza: SUP Yoga in Ibiza<\/li><\/ul>",
        "slug": "17-ibiza",
        "total_activities": 15,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/57-shrine-s320181207-4-ogiom4-1544177065.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/57-shrine-s320181207-4-ogiom4-1544177065.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/57-shrine-s320181207-4-ogiom4-1544177065.jpg"
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
              "id": "343",
              "type": "activity"
            },
            {
              "id": "358",
              "type": "activity"
            },
            {
              "id": "344",
              "type": "activity"
            },
            {
              "id": "275",
              "type": "activity"
            },
            {
              "id": "271",
              "type": "activity"
            },
            {
              "id": "276",
              "type": "activity"
            },
            {
              "id": "274",
              "type": "activity"
            },
            {
              "id": "272",
              "type": "activity"
            },
            {
              "id": "273",
              "type": "activity"
            },
            {
              "id": "345",
              "type": "activity"
            },
            {
              "id": "342",
              "type": "activity"
            },
            {
              "id": "607",
              "type": "activity"
            },
            {
              "id": "357",
              "type": "activity"
            },
            {
              "id": "348",
              "type": "activity"
            },
            {
              "id": "359",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "21",
      "type": "destination",
      "attributes": {
        "id": 21,
        "name": "Mallorca",
        "short_description": "Mallorca is the biggest island of the Balearics, and probably the most famous one as well! ",
        "description": "<div>Mallorca is the biggest island of the Balearics, and probably the most famous one as well! While most people might associate Mallorca with wild parties, cheap beer and a lot of fun, there is actually so much more to this natural paradise.&nbsp;<\/div><div>Head away from the busy touristic beaches around El Arenal and Palma de Mallorca, and you\u2019ll find idyllic vineyards in the inland, paradisical beaches all around the coast and always a quiet place to sit and simply relax. Mallorca is truly a raw diamond for all nature lovers and active travellers out there. During summer you can try all kinds of watersport activities in the warm and calm water of the Mediterranean, and the rest of the year you can go hiking, cycling, surfing running and simply explore the amazing landscapes of Mallorca.&nbsp;<\/div><div>Palma de Mallorca has also become more and more popular among celebritites and luxury-lovers, offering cute high-class boutiques and a very exquisite cuisine! Mallorca is simply an all-rounder, and the perfect destination for everybody!<\/div><div><br><\/div><ul><li>Our favorite beach: Cala Torta<\/li><li>Our favorite restaurant: Max Garden in Palmanova<\/li><li>Our favorite boat tour in Mallorca: Full day private tour in Mallorca<\/li><\/ul>",
        "slug": "21-mallorca",
        "total_activities": 2,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/61-shrine-s320181207-4-1oh2xot-1544177423.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/61-shrine-s320181207-4-1oh2xot-1544177423.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/61-shrine-s320181207-4-1oh2xot-1544177423.jpg"
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
              "id": "528",
              "type": "activity"
            },
            {
              "id": "517",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "30",
      "type": "destination",
      "attributes": {
        "id": 30,
        "name": "Tarifa",
        "short_description": "This beautiful little town in the southern tip of the Spanish mainland is a real hotspot for ocean lovers. ",
        "description": "<div>This beautiful little town in the southern tip of the Spanish mainland is a real hotspot for ocean lovers. In Tarifa, the Atlantic Ocean meets the Mediterranean Sea, and this means that you get to see A LOT of dolphins and whales. In fact, even orcas can be found off the coast of Tarifa!&nbsp;<\/div><div>The special geography also makes it the perfect spot for kitesurfing thanks to the good winds that blow here during summer. And the waves for surfing in Tarifa are also great!&nbsp;<\/div><div>The dolphin and orca watching boat tours in Tarifa are the absolute highlight though, and the cute little old town invites for a delicious lunch in one of the hip caf\u00e9s afterwards. Come and let the mix of European and North African charme enchant you in this amazing little Spanish town!<\/div><div><br><\/div><ul><li>Our favorite beach: Playa de Bolonia<\/li><li>Our favorite restaurant: Chilimosa Vegetarian Food<\/li><li>Our favorite boat tour in Tarifa: Orca Watching in Tarifa<\/li><li>Our favorite water sport in Tarifa: Kitesurfing in Tarifa&nbsp;<\/li><\/ul><div><br><br><\/div>",
        "slug": "30-tarifa",
        "total_activities": 2,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/70-shrine-s320181207-4-rimup9-1544178528.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/70-shrine-s320181207-4-rimup9-1544178528.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/70-shrine-s320181207-4-rimup9-1544178528.jpg"
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
              "id": "258",
              "type": "activity"
            },
            {
              "id": "257",
              "type": "activity"
            }
          ]
        }
      }
    },
    {
      "id": "32",
      "type": "destination",
      "attributes": {
        "id": 32,
        "name": "Tenerife",
        "short_description": "There\u2019s a reason why the biggest Canary Island has been so popular amongst travelers for the past decades. ",
        "description": "<div>There\u2019s a reason why the biggest Canary Island has been so popular amongst travelers for the past decades. The volcanic island has plenty of things to offer, from beautiful forests and nature parks to great local cuisine and a lot of different water sport activities. And of course here you\u2019ll find picturesque beaches, and of all that with a view over the Teide, Spain\u2019s highest mountain!<\/div><div>The towns of Tenerife are definitely worth a visit, especially the town of La Laguna with its beautiful historic center. Divers and those wanting to try it out will have plenty of options to choose from, since diving in Tenerife is very popular. But even if you just want to go snorkeling in Tenerife you\u2019re in for a treat, because there are a lot of sea turtles waiting to swim with you in the waters of Tenerife. Boat tours in Tenerife are a great way to discover the coastline of this fantastic island.&nbsp;<\/div><div><br><\/div><ul><li>Our favorite beach: Playa de las Vistas<\/li><li>Our favorite restaurant: Almar Tenerife<\/li><li>Our favorite boat tour in Tenerife: Submarine in Tenerife<\/li><li>Our favorite water sport in Tenerife: Scuba Diving in Tenerife<\/li><\/ul>",
        "slug": "32-tenerife",
        "total_activities": 6,
        "media": {
          "original": "http:\/\/app.sb.com:3000\/photos\/original\/72-shrine-s320181207-4-136v80c-1544178648.jpg",
          "thumbnail": "http:\/\/app.sb.com:3000\/photos\/thumbnail\/72-shrine-s320181207-4-136v80c-1544178648.jpg",
          "medium": "http:\/\/app.sb.com:3000\/photos\/medium\/72-shrine-s320181207-4-136v80c-1544178648.jpg"
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
              "id": "351",
              "type": "activity"
            },
            {
              "id": "611",
              "type": "activity"
            },
            {
              "id": "350",
              "type": "activity"
            },
            {
              "id": "596",
              "type": "activity"
            },
            {
              "id": "577",
              "type": "activity"
            },
            {
              "id": "349",
              "type": "activity"
 

```

### HTTP Request
`GET http://www.seabookings.com/api/v1/countries`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include | - | A comma separated list of all associations we wish to sideload. Allowed value is `destinations`

