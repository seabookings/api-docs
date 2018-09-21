# Activities

An activity is a tour experience. These set of endpoints allow you to get search/explore and get an experience.

The settings element will dictate much of the behaviour when performing a booking.

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
    "data": [
        {
            "id": "1",
            "type": "activity",
            "attributes": {
                "id": 1,
                "name": "Kayak tour 0",
                "description": "<div>A nice kayak tour through Benagil 0</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "1-kayak-tour-0",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 1,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/1.jpg?1535127515",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/1.jpg?1535127515"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 51.5142,
                        "lng": -0.0931
                    }
                },
                "media": [
                    {
                        "description": "barcelona-location",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "medium": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "medium": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "medium": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "thumbnail": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
                }
            },
            "relationships": {
                "tags": {
                    "data": []
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
                "description": "<div>A nice kayak tour through Benagil 1</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "2-kayak-tour-1",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 2,
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/2.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/2.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/2.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "medium": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "thumbnail": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "medium": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "medium": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "medium": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "booking_strategy": "indirect",
                "slug": "3-kayak-tour-2",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 3,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/3.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/3.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
        }
    ],
    "included": []
}
```

### HTTP Request

`GET http://www.seabookings.com/api/v1/activities/:id`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
id | - | The activity id


### Response properties

Property | Description
--------- | -----------
id | A string describing what type of activity we want to search
name | The name of the activity
description | Text describing the activity
short_description | Small text describing the activity
time zone | Time zone where the activity is located
slug | A friendly id of the activity
availability | The availability of the activity
image | The profile picture of the activity in 3 sizes
geo | The location of the activity
settings | The booking policies and properties associated with the activity

## Availability

Get the availability of an activity

```shell
curl "http://www.seabookings.com/api/v1/activities/1/availability"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/1/availability", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "type": "availability",
        "attributes": {
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
                "description": "<div>A nice kayak tour through Benagil 0</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "1-kayak-tour-0",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 1,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/1.jpg?1535127515",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/1.jpg?1535127515"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 51.5142,
                        "lng": -0.0931
                    }
                },
                "media": [
                    {
                        "description": "barcelona-location",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "medium": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "medium": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "medium": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "thumbnail": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
                }
            },
            "relationships": {
                "tags": {
                    "data": []
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
                "description": "<div>A nice kayak tour through Benagil 1</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "2-kayak-tour-1",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 2,
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/2.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/2.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/2.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "medium": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "thumbnail": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "medium": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "medium": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "medium": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "booking_strategy": "indirect",
                "slug": "3-kayak-tour-2",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 3,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/3.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/3.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 3</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "4-kayak-tour-3",
                "availability": {
                    "2018-08-27": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/4.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/4.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/4.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 4</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "5-kayak-tour-4",
                "availability": {
                    "2018-08-27": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/5.jpg",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/5.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/5.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/5.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 5</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "6-kayak-tour-5",
                "availability": {
                    "2018-08-27": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/6.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/6.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/6.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 6</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "7-kayak-tour-6",
                "availability": {
                    "2018-08-27": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/7.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/7.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/7.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 7</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "8-kayak-tour-7",
                "availability": {
                    "2018-08-27": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/8.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/8.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/8.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 8</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "9-kayak-tour-8",
                "availability": {
                    "2018-08-27": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/9.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/9.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/9.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 9</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "10-kayak-tour-9",
                "availability": {
                    "2018-08-27": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/10.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/10.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/10.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
curl "http://www.seabookings.com/api/v1/activities/explore/?tags=accessible,surf&country_code=PT&city='Benagil'"
  -H "Authorization: Bearer my_own_token"
```

```javascript
var xmlHttp = new XMLHttpRequest();
xmlHttp.open( "GET", "/api/v1/activities/explore/?tags=accessible,surf&country_code=PT&city='Benagil'", false ); // false for synchronous request
xmlHttp.send( null );
```

> The above command returns JSON structured like this:

```json
{
    "data": [
        {
            "id": "5",
            "type": "activity",
            "attributes": {
                "id": 5,
                "name": "Kayak tour 4",
                "description": "<div>A nice kayak tour through Benagil 4</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "5-kayak-tour-4",
                "availability": {
                    "2018-08-27": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-08-28": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-08-29": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-08-30": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-08-31": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-09-01": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-09-02": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ],
                    "2018-09-03": [
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
                            "num_reservations": 0,
                            "unavailable": false,
                            "reason": null,
                            "unavailability_description": null
                        }
                    ]
                },
                "image": {
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/5.jpg",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/5.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/5.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/5.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
            "id": "10",
            "type": "activity",
            "attributes": {
                "id": 10,
                "name": "Kayak tour 9",
                "description": "<div>A nice kayak tour through Benagil 9</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "10-kayak-tour-9",
                "availability": {
                    "2018-08-27": [
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
                    ],
                    "2018-08-28": [
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
                    ],
                    "2018-08-29": [
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
                    ],
                    "2018-08-30": [
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
                    ],
                    "2018-08-31": [
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
                    ],
                    "2018-09-01": [
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
                    ],
                    "2018-09-02": [
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
                    ],
                    "2018-09-03": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/10.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/10.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/10.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
        },
        {
            "id": "6",
            "type": "activity",
            "attributes": {
                "id": 6,
                "name": "Kayak tour 5",
                "description": "<div>A nice kayak tour through Benagil 5</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "6-kayak-tour-5",
                "availability": {
                    "2018-08-27": [
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
                    ],
                    "2018-08-28": [
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
                    ],
                    "2018-08-29": [
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
                    ],
                    "2018-08-30": [
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
                    ],
                    "2018-08-31": [
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
                    ],
                    "2018-09-01": [
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
                    ],
                    "2018-09-02": [
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
                    ],
                    "2018-09-03": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/6.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/6.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/6.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 0,
                        "lng": 0
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "description": "<div>A nice kayak tour through Benagil 6</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "7-kayak-tour-6",
                "availability": {
                    "2018-08-27": [
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
                    ],
                    "2018-08-28": [
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
                    ],
                    "2018-08-29": [
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
                    ],
                    "2018-08-30": [
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
                    ],
                    "2018-08-31": [
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
                    ],
                    "2018-09-01": [
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
                    ],
                    "2018-09-02": [
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
                    ],
                    "2018-09-03": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/7.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/7.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/7.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
            "id": "2",
            "type": "activity",
            "attributes": {
                "id": 2,
                "name": "Kayak tour 1",
                "description": "<div>A nice kayak tour through Benagil 1</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "2-kayak-tour-1",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 2,
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
                    ],
                    "2018-08-28": [
                        {
                            "slot_id": 2,
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
                    ],
                    "2018-08-29": [
                        {
                            "slot_id": 2,
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
                    ],
                    "2018-08-30": [
                        {
                            "slot_id": 2,
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
                    ],
                    "2018-08-31": [
                        {
                            "slot_id": 2,
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
                    ],
                    "2018-09-01": [
                        {
                            "slot_id": 2,
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
                    ],
                    "2018-09-02": [
                        {
                            "slot_id": 2,
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
                    ],
                    "2018-09-03": [
                        {
                            "slot_id": 2,
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/2.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/2.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/2.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "medium": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "thumbnail": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "medium": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "medium": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "medium": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "booking_strategy": "indirect",
                "slug": "3-kayak-tour-2",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 3,
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
                    ],
                    "2018-08-28": [
                        {
                            "slot_id": 3,
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
                    ],
                    "2018-08-29": [
                        {
                            "slot_id": 3,
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
                    ],
                    "2018-08-30": [
                        {
                            "slot_id": 3,
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
                    ],
                    "2018-08-31": [
                        {
                            "slot_id": 3,
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
                    ],
                    "2018-09-01": [
                        {
                            "slot_id": 3,
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
                    ],
                    "2018-09-02": [
                        {
                            "slot_id": 3,
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
                    ],
                    "2018-09-03": [
                        {
                            "slot_id": 3,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/3.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/3.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
            "id": "8",
            "type": "activity",
            "attributes": {
                "id": 8,
                "name": "Kayak tour 7",
                "description": "<div>A nice kayak tour through Benagil 7</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "8-kayak-tour-7",
                "availability": {
                    "2018-08-27": [
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
                    ],
                    "2018-08-28": [
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
                    ],
                    "2018-08-29": [
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
                    ],
                    "2018-08-30": [
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
                    ],
                    "2018-08-31": [
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
                    ],
                    "2018-09-01": [
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
                    ],
                    "2018-09-02": [
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
                    ],
                    "2018-09-03": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/8.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/8.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/8.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
            "id": "4",
            "type": "activity",
            "attributes": {
                "id": 4,
                "name": "Kayak tour 3",
                "description": "<div>A nice kayak tour through Benagil 3</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "4-kayak-tour-3",
                "availability": {
                    "2018-08-27": [
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
                    ],
                    "2018-08-28": [
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
                    ],
                    "2018-08-29": [
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
                    ],
                    "2018-08-30": [
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
                    ],
                    "2018-08-31": [
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
                    ],
                    "2018-09-01": [
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
                    ],
                    "2018-09-02": [
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
                    ],
                    "2018-09-03": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/4.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/4.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/4.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
            "id": "9",
            "type": "activity",
            "attributes": {
                "id": 9,
                "name": "Kayak tour 8",
                "description": "<div>A nice kayak tour through Benagil 8</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "9-kayak-tour-8",
                "availability": {
                    "2018-08-27": [
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
                    ],
                    "2018-08-28": [
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
                    ],
                    "2018-08-29": [
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
                    ],
                    "2018-08-30": [
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
                    ],
                    "2018-08-31": [
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
                    ],
                    "2018-09-01": [
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
                    ],
                    "2018-09-02": [
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
                    ],
                    "2018-09-03": [
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/9.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/9.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/9.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
            "id": "1",
            "type": "activity",
            "attributes": {
                "id": 1,
                "name": "Kayak tour 0",
                "description": "<div>A nice kayak tour through Benagil 0</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "1-kayak-tour-0",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 1,
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
                    ],
                    "2018-08-28": [
                        {
                            "slot_id": 1,
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
                    ],
                    "2018-08-29": [
                        {
                            "slot_id": 1,
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
                    ],
                    "2018-08-30": [
                        {
                            "slot_id": 1,
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
                    ],
                    "2018-08-31": [
                        {
                            "slot_id": 1,
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
                    ],
                    "2018-09-01": [
                        {
                            "slot_id": 1,
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
                    ],
                    "2018-09-02": [
                        {
                            "slot_id": 1,
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
                    ],
                    "2018-09-03": [
                        {
                            "slot_id": 1,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/1.jpg?1535127515",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/1.jpg?1535127515"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 51.5142,
                        "lng": -0.0931
                    }
                },
                "media": [
                    {
                        "description": "barcelona-location",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "medium": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "medium": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "medium": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "thumbnail": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
                }
            },
            "relationships": {
                "tags": {
                    "data": []
                }
            },
            "links": {
                "self": "/api/v1/activities/1-kayak-tour-0"
            }
        }
    ],
    "included": [],
    "links": {
        "current_page": 1,
        "next_page": null,
        "prev_page": null,
        "current_page_url": "http://www.sb.com:3000/api/v1/activities/explore?city=Benagil",
        "next_page_url": null,
        "previous_page_url": null,
        "total_pages": 1,
        "total_count": 10
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

## Featured activities

```shell
curl -X GET \
  http://www.seabookings.com/api/v1/activities/featured \
  -H 'Authorization: Bearer dev_token' \
  -H 'Cache-Control: no-cache' \
  -H 'Postman-Token: 2940f50b-8577-4b6d-8f27-bba526965016'
```

```javascript
var data = null;

var xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === 4) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "http://www.seabookings.com/api/v1/activities/featured");
xhr.setRequestHeader("Authorization", "Bearer dev_token");
xhr.setRequestHeader("Cache-Control", "no-cache");
xhr.setRequestHeader("Postman-Token", "33b5a314-368e-4fd2-99b8-91ae3f4d6db5");

xhr.send(data);
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
                "description": "<div>A nice kayak tour through Benagil 0</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "1-kayak-tour-0",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 1,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/1.jpg?1535127515",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/1.jpg?1535127515",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/1.jpg?1535127515"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 51.5142,
                        "lng": -0.0931
                    }
                },
                "media": [
                    {
                        "description": "barcelona-location",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "medium": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/33-barcelona-location-1535369039.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "medium": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/35-barcelona-1535384203.jpg"
                        }
                    },
                    {
                        "description": "",
                        "images": {
                            "original": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "medium": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png",
                            "thumbnail": "http://sb.com:3000/photos/original/36-aws-logo-1535384269.png"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
                }
            },
            "relationships": {
                "tags": {
                    "data": []
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
                "description": "<div>A nice kayak tour through Benagil 1</div>",
                "short_description": null,
                "time_zone": "Lisbon",
                "booking_strategy": "indirect",
                "slug": "2-kayak-tour-1",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 2,
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
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/2.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/2.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/2.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "medium": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png",
                            "thumbnail": "http://sb.com:3000/photos/original/13-aws-logo-1535111814.png"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "medium": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/14-barcelona-1535111815.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "medium": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/15-boat-tour-1535111816.jpg"
                        }
                    },
                    {
                        "description": null,
                        "images": {
                            "original": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "medium": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg",
                            "thumbnail": "http://sb.com:3000/photos/original/16-Boat-trips-1535111920.jpg"
                        }
                    }
                ],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
                "booking_strategy": "indirect",
                "slug": "3-kayak-tour-2",
                "availability": {
                    "2018-08-27": [
                        {
                            "slot_id": 3,
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
                    "thumb": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "thumbnail": "http://www.sb.com:3000/uploads/1/activities/pictures/thumb/3.jpg",
                    "medium": "http://www.sb.com:3000/uploads/1/activities/pictures/medium/3.jpg",
                    "original": "http://www.sb.com:3000/uploads/1/activities/pictures/original/3.jpg"
                },
                "category": "experience",
                "geo": {
                    "country": "Portugal",
                    "city": "Benagil",
                    "full_street_address": "Praia de Benagil",
                    "coord": {
                        "lat": 38.7167,
                        "lng": -9.1333
                    }
                },
                "media": [],
                "settings": {
                    "comission_percentage": 0.2,
                    "payment_policy": "full_amount",
                    "booking_strategy": "indirect",
                    "merchant_id": "acct_19S93eBFHEM5ipEo"
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
        }
    ],
    "included": []
}
```

### HTTP Request
`GET http://www.seabookings.com/api/v1/activities/featured`

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
        "current_page_url": "http://www.seabookings.com/api/v1/activities/1/slots",
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
        "current_page_url": "http://www.seabookings.com/api/v1/activities/1/slots?include=prices",
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
        "current_page_url": "http://www.seabookings.com/api/v1/activities/1/prices",
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
