---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  - javascript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/lord/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the SeaBookings API!
You can use our API to access SeaBookings public data, which can get you information on tour activities.
At the moment we provide facilities to:

* Explore tour activities
* See the details of tour activities
* Search for a tour activity

In the near future you will be able to create reservations, and make payments.

# Authentication

> To authorize, we currently use a JWT strategy.


```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: Bearer my_own_token"
```

```javascript
// make the request to the login endpoint

function getToken() {
  var xmlHttp = new XMLHttpRequest();
  xmlHttp.open( "GET", "/api/v1/auth/anonymous/token", false ); // false for synchronous request
  xmlHttp.send( null );
  return JSON.parse(xmlHttp.responseText).token;
}

var token = getToken();
var xhr = new XMLHttpRequest();
var xhr.setRequestHeader("Authorization", "Bearer " + token);

// Then select an api endpoint and send the request

```

> Make sure to replace `my_own_token` with your JSON Web Token.

SeaBookings uses JWT to allow access to the API. You can get an anonymous token by making a request to `/api/v1/auth/anonymous/token`

SeaBookings expects for the JWT key to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer my_own_token`

<aside class="notice">
You must replace <code>my_own_token</code> with your personal JWT.
</aside>

# Activities

## Search

```shell
curl "http://www.seabookings.com/api/v1/activities/search?query=Kayak"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/search?query=Kayak", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            "id": "1",
            "type": "activity",
            "attributes": {
                "id": 1,
                "name": "Kayak tour 0",
                "description": "<div>A nice kayak tour through Benagil 1</div>",
                "short_description": "Uma descrição breve",
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "1-kayak-tour-0",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 121,
                            "start_time": "2000-01-01T17:00:00.000Z",
                            "finish_time": "2000-01-01T18:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 123,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/1.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/1.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 39.4614992,
                        "lng": -8.1994587
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": [
                        {
                            "id": "11",
                            "type": "tag"
                        },
                        {
                            "id": "13",
                            "type": "tag"
                        },
                        {
                            "id": "3",
                            "type": "tag"
                        },
                        {
                            "id": "4",
                            "type": "tag"
                        }
                    ]
                }
            },
            "links": {
                "self": "/api/v1/activities/1-kayak-tour-0"
            }
        },
        {
            "id": "2",
            "type": "activity",
            "attributes": {
                "id": 2,
                "name": "Kayak tour 1",
                "description": "A nice kayak tour through Benagil 1",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "2-kayak-tour-1",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 108,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/2.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/2.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/2.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/2-kayak-tour-1"
            }
        },
        {
            "id": "3",
            "type": "activity",
            "attributes": {
                "id": 3,
                "name": "Kayak tour 2",
                "description": "<div>A nice kayak tour through Benagil 2</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "instant",
                "slug": "3-kayak-tour-2",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 115,
                            "start_time": "2000-01-01T23:00:00.000Z",
                            "finish_time": "2000-01-01T23:12:00.000Z",
                            "duration": 720,
                            "duration_unit": "seconds",
                            "capacity": 1,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/3.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/3.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 39.8085,
                        "lng": -8.0988
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/3-kayak-tour-2"
            }
        },
        {
            "id": "4",
            "type": "activity",
            "attributes": {
                "id": 4,
                "name": "Kayak tour 3",
                "description": "A nice kayak tour through Benagil 3",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "4-kayak-tour-3",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 4,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/4.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/4.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/4.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/4-kayak-tour-3"
            }
        },
        {
            "id": "5",
            "type": "activity",
            "attributes": {
                "id": 5,
                "name": "Kayak tour 4",
                "description": "A nice kayak tour through Benagil 4",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "5-kayak-tour-4",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 5,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 1,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/5.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/5.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/5.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/5-kayak-tour-4"
            }
        },
        {
            "id": "6",
            "type": "activity",
            "attributes": {
                "id": 6,
                "name": "Kayak tour 5",
                "description": "A nice kayak tour through Benagil 5",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "6-kayak-tour-5",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 6,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/6.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/6.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/6.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/6-kayak-tour-5"
            }
        },
        {
            "id": "7",
            "type": "activity",
            "attributes": {
                "id": 7,
                "name": "Kayak tour 6",
                "description": "A nice kayak tour through Benagil 6",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "7-kayak-tour-6",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 7,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/7.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/7.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/7.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/7-kayak-tour-6"
            }
        },
        {
            "id": "8",
            "type": "activity",
            "attributes": {
                "id": 8,
                "name": "Kayak tour 7",
                "description": "A nice kayak tour through Benagil 7",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "8-kayak-tour-7",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 8,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/8.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/8.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/8.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/8-kayak-tour-7"
            }
        },
        {
            "id": "9",
            "type": "activity",
            "attributes": {
                "id": 9,
                "name": "Kayak tour 8",
                "description": "A nice kayak tour through Benagil 8",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "9-kayak-tour-8",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 9,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/9.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/9.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/9.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/9-kayak-tour-8"
            }
        },
        {
            "id": "10",
            "type": "activity",
            "attributes": {
                "id": 10,
                "name": "Kayak tour 9",
                "description": "A nice kayak tour through Benagil 9",
                "short_description": null,
                "time_zone": "Europe/Lisbon",
                "booking_strategy": "instant",
                "slug": "10-kayak-tour-9",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 10,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 20,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 0,
                                "seconds": 0
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/10.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/10.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/10.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/10-kayak-tour-9"
            }
        }
    ],
    "links": {
        "current_page": 1,
        "next_page": null,
        "prev_page": null,
        "current_page_url": "http://www.sb.com:3000/api/v1/activities/search?query=Kayak",
        "next_page_url": null,
        "previous_page_url": null,
        "total_pages": 1,
        "total_count": 10
    }
}

```

### HTTP Request

`GET http://www.seabookings.com/api/v1/activities/search?query=:query`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
query | - | A string describing what type of activity we want to search
location | - | The location of the activity, specified by city and country, ex: "Lagos Portugal"
distance | - | A number indicating the maximum distance radius to the location (Requires location to be set)
distance_unit | km | The unit of the distance (Requires location and distance to be set)


## Explore

```shell
curl "http://www.seabookings.com/api/v1/activities/explore/?tags=accessible,surf&country_code=PT&city_slug='Lagos'"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/explore/?tags=accessible,surf&country_code=PT&city_slug='Lagos'", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            "id": "13",
            "type": "activity",
            "attributes": {
                "id": 13,
                "name": "a Barcelona experience",
                "description": "<div>asdasdasdas<br>asdas<br>das<br>das<br>das<br>das<br>das<br><br></div>",
                "short_description": "asd",
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "13-a-barcelona-experience",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 112,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 1,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 2520,
                                "seconds": 151200
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-24": [
                        {
                            "slot_id": 112,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 1,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 2520,
                                "seconds": 151200
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-25": [
                        {
                            "slot_id": 112,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 1,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 2520,
                                "seconds": 151200
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-26": [
                        {
                            "slot_id": 112,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 1,
                            "starting_price_cents": 1000,
                            "cutoff": {
                                "minutes": 2520,
                                "seconds": 151200
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-27": [],
                    "2018-07-28": [],
                    "2018-07-29": [],
                    "2018-07-30": []
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/2/activities/pictures/thumb/13.jpg?1530630839",
                    "medium": "http://www.sb.com:3000/uploads/2/activities/pictures/medium/13.jpg?1530630839",
                    "original": "http://www.sb.com:3000/uploads/2/activities/pictures/original/13.jpg?1530630839"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Lisbon",
                    "coord": {
                        "lat": 51.4964,
                        "lng": -0.1224
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": [
                        {
                            "id": "8",
                            "type": "tag"
                        },
                        {
                            "id": "12",
                            "type": "tag"
                        },
                        {
                            "id": "11",
                            "type": "tag"
                        }
                    ]
                }
            },
            "links": {
                "self": "/api/v1/activities/13-a-barcelona-experience"
            }
        },
        {
            "id": "1",
            "type": "activity",
            "attributes": {
                "id": 1,
                "name": "Kayak tour 0",
                "description": "<div>A nice kayak tour through Benagil 1</div>",
                "short_description": "Uma descrição breve",
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "1-kayak-tour-0",
                "availability": {
                    "2018-07-23": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 121,
                            "start_time": "2000-01-01T17:00:00.000Z",
                            "finish_time": "2000-01-01T18:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 123,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-24": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 121,
                            "start_time": "2000-01-01T17:00:00.000Z",
                            "finish_time": "2000-01-01T18:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 123,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-25": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 121,
                            "start_time": "2000-01-01T17:00:00.000Z",
                            "finish_time": "2000-01-01T18:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 123,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-26": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-27": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-28": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-29": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 104,
                            "start_time": "2000-01-01T18:00:00.000Z",
                            "finish_time": "2000-01-01T19:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 22,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-07-30": [
                        {
                            "slot_id": 120,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 18000,
                            "duration_unit": "seconds",
                            "capacity": 10,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 122,
                            "start_time": "2000-01-01T09:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 10800,
                            "duration_unit": "seconds",
                            "capacity": 11,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 97,
                            "start_time": "2000-01-01T10:00:00.000Z",
                            "finish_time": "2000-01-01T12:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 2,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 119,
                            "start_time": "2000-01-01T13:00:00.000Z",
                            "finish_time": "2000-01-01T14:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 89,
                            "start_time": "2000-01-01T15:00:00.000Z",
                            "finish_time": "2000-01-01T17:00:00.000Z",
                            "duration": 7200,
                            "duration_unit": "seconds",
                            "capacity": 12,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        },
                        {
                            "slot_id": 102,
                            "start_time": "2000-01-01T19:00:00.000Z",
                            "finish_time": "2000-01-01T20:00:00.000Z",
                            "duration": 3600,
                            "duration_unit": "seconds",
                            "capacity": 128,
                            "starting_price_cents": 2000,
                            "cutoff": {
                                "minutes": 1440,
                                "seconds": 86400
                            },
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/1.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/1.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "coord": {
                        "lat": 39.4614992,
                        "lng": -8.1994587
                    }
                },
                "settings": {
                    "deposit_percentage": 0.2
                }
            },
            "relationships": {
                "tags": {
                    "data": [
                        {
                            "id": "11",
                            "type": "tag"
                        },
                        {
                            "id": "13",
                            "type": "tag"
                        },
                        {
                            "id": "3",
                            "type": "tag"
                        },
                        {
                            "id": "4",
                            "type": "tag"
                        }
                    ]
                }
            },
            "links": {
                "self": "/api/v1/activities/1-kayak-tour-0"
            }
        }
    ],
    "included": [
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
            "id": "12",
            "type": "tag",
            "attributes": {
                "id": 12,
                "key": "children_safe",
                "label": "Children safe"
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
            "id": "13",
            "type": "tag",
            "attributes": {
                "id": 13,
                "key": "party_boat",
                "label": "Party boat"
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
        }
    ],
    "links": {
        "current_page": 1,
        "next_page": null,
        "prev_page": null,
        "current_page_url": "http://www.sb.com:3000/api/v1/activities/explore?tags=accessible&country_code=PT",
        "next_page_url": null,
        "previous_page_url": null,
        "total_pages": 1,
        "total_count": 2
    }
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/activities/explore/?tags=:tags&country_code=:country_code&city_slug=:city_slug`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
tags | - | A comma separated list of all tags that we wish that the results include
country_code | - | The country Code we wish to filter (Currently available countries are: PT for Portugal, ES for Spain)
city_slug | - | The slug associated with the city we wish to filter from

## Get a single activity

```shell
curl "http://www.seabookings.com/api/v1/activities/1"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/1" ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "id": "1",
    "type": "activity",
    "attributes": {
      "id": 1,
      "name": "Kayak tour 0",
      "description": "<div>A nice kayak tour through Benagil 0</div>",
      "time_zone": "Lisbon",
      "booking_strategy": "instant",
      "slug": "1-kayak-tour-0",
      "image": {
        "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg",
        "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/1.jpg",
        "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/1.jpg"
      },
      "category": "experience",
      "geo": {
        "country": "Portugal",
        "city": "Benagil",
        "coord": {
          "lat": "37.0887105",
          "lng": "-8.4311101"
        }
      }
    },
    "relationships": {
      "tags": {
        "data": [{
          "id": "11",
          "type": "tag"
        }]
      }
    },
    "links": {
      "self": "/api/v1/activities/1-kayak-tour-0"
    }
  },
  "included": [{
    "id": "11",
    "type": "tag",
    "attributes": {
      "id": 11,
      "key": "accessible",
      "label": "Accessible"
    }
  }]
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/activities/:id`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
id | - | The activity id

## Availability

Get the availability of an activity

```shell
curl "http://www.seabookings.com/api/v1/activities/1/availability"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/availability", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "type": "availability",
        "attributes": {
            "2018-07-11": [
                {
                    "slot_id": 95,
                    "start_time": "2000-01-01T09:00:00.000Z",
                    "finish_time": "2000-01-01T14:00:00.000Z",
                    "duration": 18000,
                    "duration_unit": "seconds",
                    "capacity": 10,
                    "starting_price_cents": 2000,
                    "num_reservations": 0,
                    "unavailable": false,
                    "reason": null,
                    "unavailability_description": null
                },
                {
                    "slot_id": 97,
                    "start_time": "2000-01-01T10:00:00.000Z",
                    "finish_time": "2000-01-01T12:00:00.000Z",
                    "duration": 7200,
                    "duration_unit": "seconds",
                    "capacity": 2,
                    "starting_price_cents": 2000,
                    "num_reservations": 0,
                    "unavailable": false,
                    "reason": null,
                    "unavailability_description": null
                },
                {
                    "slot_id": 99,
                    "start_time": "2000-01-01T13:00:00.000Z",
                    "finish_time": "2000-01-01T14:00:00.000Z",
                    "duration": 3600,
                    "duration_unit": "seconds",
                    "capacity": 12,
                    "starting_price_cents": 2000,
                    "num_reservations": 0,
                    "unavailable": false,
                    "reason": null,
                    "unavailability_description": null
                },
                {
                    "slot_id": 89,
                    "start_time": "2000-01-01T15:00:00.000Z",
                    "finish_time": "2000-01-01T17:00:00.000Z",
                    "duration": 7200,
                    "duration_unit": "seconds",
                    "capacity": 12,
                    "starting_price_cents": 2000,
                    "num_reservations": 0,
                    "unavailable": false,
                    "reason": null,
                    "unavailability_description": null
                },
                {
                    "slot_id": 91,
                    "start_time": "2000-01-01T17:00:00.000Z",
                    "finish_time": "2000-01-01T18:00:00.000Z",
                    "duration": 3600,
                    "duration_unit": "seconds",
                    "capacity": 123,
                    "starting_price_cents": 2000,
                    "num_reservations": 0,
                    "unavailable": false,
                    "reason": null,
                    "unavailability_description": null
                },
                {
                    "slot_id": 104,
                    "start_time": "2000-01-01T18:00:00.000Z",
                    "finish_time": "2000-01-01T19:00:00.000Z",
                    "duration": 3600,
                    "duration_unit": "seconds",
                    "capacity": 22,
                    "starting_price_cents": 2000,
                    "num_reservations": 0,
                    "unavailable": false,
                    "reason": null,
                    "unavailability_description": null
                },
                {
                    "slot_id": 102,
                    "start_time": "2000-01-01T19:00:00.000Z",
                    "finish_time": "2000-01-01T20:00:00.000Z",
                    "duration": 3600,
                    "duration_unit": "seconds",
                    "capacity": 128,
                    "starting_price_cents": 2000,
                    "num_reservations": 0,
                    "unavailable": false,
                    "reason": null,
                    "unavailability_description": null
                }
            ]
        }
    }
}
```
### HTTP Request

`GET http://www.seabookings.com/api/v1/activities/:id/availability`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
start_date | today | Lower date limit for availability lookup
end_date | today | Upper date limit for availability lookup

## Slots

Get all slots of an activity

```shell
curl "http://www.seabookings.com/api/v1/activities/1/slots"
  -H "Authorization: Bearer my_own_token"
```

> You can include the prices in the response by passing the parameter `include=prices`

```shell
curl "http://www.seabookings.com/api/v1/activities/1/slots?include=prices"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/1/slots", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            "id": "14",
            "type": "slot",
            "attributes": {
                "id": 14,
                "start_at": "2018-04-01",
                "finish_at": "2018-12-31",
                "start_time": "2000-01-01T09:00:00.000Z",
                "finish_time": "2000-01-01T12:00:00.000Z",
                "capacity": 20,
                "cutoff_minutes": 0,
                "deleted_at": "2018-04-03T00:00:00.000Z",
                "created_at": "2018-03-30T15:03:16.356Z",
                "updated_at": "2018-04-03T11:38:00.819Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "1",
                            "type": "price"
                        },
                        {
                            "id": "2",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "99",
            "type": "slot",
            "attributes": {
                "id": 99,
                "start_at": "2018-06-27",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T13:00:00.000Z",
                "finish_time": "2000-01-01T14:00:00.000Z",
                "capacity": 12,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-29T08:27:59.482Z",
                "updated_at": "2018-07-06T13:43:38.322Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "2",
                            "type": "price"
                        },
                        {
                            "id": "21",
                            "type": "price"
                        },
                        {
                            "id": "22",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "95",
            "type": "slot",
            "attributes": {
                "id": 95,
                "start_at": "2018-06-28",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T09:00:00.000Z",
                "finish_time": "2000-01-01T14:00:00.000Z",
                "capacity": 10,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-29T08:27:15.060Z",
                "updated_at": "2018-06-29T08:27:15.065Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "25",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "89",
            "type": "slot",
            "attributes": {
                "id": 89,
                "start_at": "2018-06-15",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T15:00:00.000Z",
                "finish_time": "2000-01-01T17:00:00.000Z",
                "capacity": 12,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-14T11:26:06.123Z",
                "updated_at": "2018-06-15T15:46:43.678Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "2",
                            "type": "price"
                        },
                        {
                            "id": "21",
                            "type": "price"
                        },
                        {
                            "id": "22",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "102",
            "type": "slot",
            "attributes": {
                "id": 102,
                "start_at": "2018-06-29",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T19:00:00.000Z",
                "finish_time": "2000-01-01T20:00:00.000Z",
                "capacity": 128,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-29T08:32:41.992Z",
                "updated_at": "2018-06-29T08:32:42.013Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "2",
                            "type": "price"
                        },
                        {
                            "id": "21",
                            "type": "price"
                        },
                        {
                            "id": "22",
                            "type": "price"
                        }
                    ]
                }
            }
        }
    ],
    "links": {
        "current_page": 1,
        "next_page": 2,
        "prev_page": null,
        "current_page_url": "http://www.sb.com:3000/api/v1/activities/1/slots",
        "next_page_url": "/api/v1/activities/1/slots?page=2",
        "previous_page_url": null,
        "total_pages": 2,
        "total_count": 8
    }
}
```

> With the prices included the returned response is

```json
{
    "data": [
        {
            "id": "14",
            "type": "slot",
            "attributes": {
                "id": 14,
                "start_at": "2018-04-01",
                "finish_at": "2018-12-31",
                "start_time": "2000-01-01T09:00:00.000Z",
                "finish_time": "2000-01-01T12:00:00.000Z",
                "capacity": 20,
                "cutoff_minutes": 0,
                "deleted_at": "2018-04-03T00:00:00.000Z",
                "created_at": "2018-03-30T15:03:16.356Z",
                "updated_at": "2018-04-03T11:38:00.819Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "1",
                            "type": "price"
                        },
                        {
                            "id": "2",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "99",
            "type": "slot",
            "attributes": {
                "id": 99,
                "start_at": "2018-06-27",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T13:00:00.000Z",
                "finish_time": "2000-01-01T14:00:00.000Z",
                "capacity": 12,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-29T08:27:59.482Z",
                "updated_at": "2018-07-06T13:43:38.322Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "2",
                            "type": "price"
                        },
                        {
                            "id": "21",
                            "type": "price"
                        },
                        {
                            "id": "22",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "95",
            "type": "slot",
            "attributes": {
                "id": 95,
                "start_at": "2018-06-28",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T09:00:00.000Z",
                "finish_time": "2000-01-01T14:00:00.000Z",
                "capacity": 10,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-29T08:27:15.060Z",
                "updated_at": "2018-06-29T08:27:15.065Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "25",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "89",
            "type": "slot",
            "attributes": {
                "id": 89,
                "start_at": "2018-06-15",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T15:00:00.000Z",
                "finish_time": "2000-01-01T17:00:00.000Z",
                "capacity": 12,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-14T11:26:06.123Z",
                "updated_at": "2018-06-15T15:46:43.678Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "2",
                            "type": "price"
                        },
                        {
                            "id": "21",
                            "type": "price"
                        },
                        {
                            "id": "22",
                            "type": "price"
                        }
                    ]
                }
            }
        },
        {
            "id": "102",
            "type": "slot",
            "attributes": {
                "id": 102,
                "start_at": "2018-06-29",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T19:00:00.000Z",
                "finish_time": "2000-01-01T20:00:00.000Z",
                "capacity": 128,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-06-29T08:32:41.992Z",
                "updated_at": "2018-06-29T08:32:42.013Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "2",
                            "type": "price"
                        },
                        {
                            "id": "21",
                            "type": "price"
                        },
                        {
                            "id": "22",
                            "type": "price"
                        }
                    ]
                }
            }
        }
    ],
    "included": [
        {
            "id": "1",
            "type": "price",
            "attributes": {
                "id": 1,
                "value_cents": 1000,
                "num_individuals": 1,
                "label": "Adults",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "2",
            "type": "price",
            "attributes": {
                "id": 2,
                "value_cents": 2000,
                "num_individuals": 1,
                "label": "Groups",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "21",
            "type": "price",
            "attributes": {
                "id": 21,
                "value_cents": 1000,
                "num_individuals": 4,
                "label": "Families",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "22",
            "type": "price",
            "attributes": {
                "id": 22,
                "value_cents": 1000,
                "num_individuals": 1,
                "label": "Adults",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "25",
            "type": "price",
            "attributes": {
                "id": 25,
                "value_cents": 2000,
                "num_individuals": 1,
                "label": "Groups",
                "min_age": null,
                "max_age": null
            }
        }
    ],
    "links": {
        "current_page": 1,
        "next_page": 2,
        "prev_page": null,
        "current_page_url": "http://www.sb.com:3000/api/v1/activities/1/slots?include=prices",
        "next_page_url": "/api/v1/activities/1/slots?include=prices&page=2",
        "previous_page_url": null,
        "total_pages": 2,
        "total_count": 8
    }
} 
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/activities/:id/slots`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
slot_ids | - | A comma separated list of all slots ids that we wish to retrieve. If this parameter is passed, start_date and end_date parameters are ignored.
start_date | today | A date to start looking for enabled time slots
end_date | today | The date until we look for enabled time slots
include | - | This endpoint allows the sideload of prices. For that pass the parameter `include` with value `prices`


## Prices

Get all prices of an activity

```shell
curl "http://www.seabookings.com/api/v1/activities/1/prices"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/prices", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            "id": "22",
            "type": "price",
            "attributes": {
                "id": 22,
                "value_cents": 1000,
                "num_individuals": 1,
                "label": "Adults",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "1",
            "type": "price",
            "attributes": {
                "id": 1,
                "value_cents": 1000,
                "num_individuals": 1,
                "label": "Adults",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "24",
            "type": "price",
            "attributes": {
                "id": 24,
                "value_cents": 1000,
                "num_individuals": 1,
                "label": "Adults",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "2",
            "type": "price",
            "attributes": {
                "id": 2,
                "value_cents": 2000,
                "num_individuals": 1,
                "label": "Groups",
                "min_age": null,
                "max_age": null
            }
        },
        {
            "id": "21",
            "type": "price",
            "attributes": {
                "id": 21,
                "value_cents": 1000,
                "num_individuals": 4,
                "label": "Families",
                "min_age": null,
                "max_age": null
            }
        }
    ],
    "links": {
        "current_page": 1,
        "next_page": 2,
        "prev_page": null,
        "current_page_url": "http://www.sb.com:3000/api/v1/activities/1/prices",
        "next_page_url": "/api/v1/activities/1/prices?page=2",
        "previous_page_url": null,
        "total_pages": 2,
        "total_count": 6
    }
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/activities/:id/prices`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
price_ids | - | A comma separated list of all price ids that we wish to retrieve. If nothing is submitted all prices are returned.

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

