# Bookings

## Create Booking

```shell
curl -X POST \
  http://www.sb.com:3000/api/v1/bookings \
  -H 'Authorization: Bearer dev_token' \
  -H 'Cache-Control: no-cache' \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: 66cd4953-fd98-4d8a-b54a-880d68d42df0' \
  -H 'Referer: www.seabookings.com' \
  -H 'User-Agent: SBPORTAL' \
  -d '{
	"activity_id": 1,
	"slot_id": 4896,
	"reservation_date": "2018-07-28",
	"customer": {
	  "name": "Test User",
	  "email": "test@domain.com",
	  "country_code": "351",
	  "phone_number": "967111111"
	},

    "price_fields": [{ "price_id": 42, "num_instances": 1 }],
	"terms_of_service": true
}'

```

```javascript
var data = JSON.stringify({
  "activity_id": 1,
  "slot_id": 5942,
  "reservation_date": "2018-07-28",
  "customer": {
    "name": "Test User",
    "email": "test@domain.com",
    "country_code": "351",
    "phone_number": "967111111"
  },
  "price_fields": [
    {
      "price_id": 42,
      "num_instances": 1
    }
  ],
  "terms_of_service": true
});

var xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === 4) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "http://www.sb.com:3000/api/v1/bookings");
xhr.setRequestHeader("User-Agent", "SBPORTAL");
xhr.setRequestHeader("Referer", "www.seabookings.com");
xhr.setRequestHeader("Content-Type", "application/json");
xhr.setRequestHeader("Authorization", "Bearer dev_token");
xhr.setRequestHeader("Cache-Control", "no-cache");
xhr.setRequestHeader("Postman-Token", "4ad189f0-a0cb-4b02-b86d-275011bdb006");

xhr.send(data);
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": "18674",
        "type": "booking",
        "attributes": {
            "reservation_date": "2018-07-28",
            "pnr": "DZR5RN",
            "created_at": "2018-07-27T17:28:25.676Z",
            "aggregated_total_cents": 1000,
            "price_total_cents": 1000,
            "application_fee_cents": 200,
            "status": "pending",
            "payment_status": "pending",
            "via": "web_public",
            "customer_note": null,
            "deposit_cents": 1000,
            "price_fields": [
                {
                    "price_id": 42,
                    "num_instances": 1,
                    "label": "Adultos"
                }
            ]
        },
        "relationships": {
            "slot": {
                "data": {
                    "id": "4896",
                    "type": "slot"
                }
            },
            "customer": {
                "data": {
                    "id": "13566",
                    "type": "customer"
                }
            }
        }
    },
    "included": [
        {
            "id": "13566",
            "type": "customer",
            "attributes": {
                "name": "Test User",
                "email": "test@domain.com",
                "country_code": "351",
                "phone_number": "967111111"
            }
        },
        {
            "id": "4896",
            "type": "slot",
            "attributes": {
                "id": 4896,
                "start_at": "2018-07-03",
                "finish_at": "2018-07-31",
                "start_time": "2000-01-01T09:00:00.000Z",
                "finish_time": "2000-01-01T12:00:00.000Z",
                "capacity": 12,
                "cutoff_minutes": 15,
                "deleted_at": null,
                "created_at": "2018-07-03T13:49:28.005Z",
                "updated_at": "2018-07-27T17:28:25.728Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "236",
                            "type": "price"
                        },
                        {
                            "id": "42",
                            "type": "price"
                        },
                        {
                            "id": "86",
                            "type": "price"
                        },
                        {
                            "id": "14",
                            "type": "price"
                        },
                        {
                            "id": "224",
                            "type": "price"
                        },
                        {
                            "id": "62",
                            "type": "price"
                        },
                        {
                            "id": "400",
                            "type": "price"
                        },
                        {
                            "id": "401",
                            "type": "price"
                        },
                        {
                            "id": "801",
                            "type": "price"
                        }
                    ]
                }
            }
        }
    ]
}
```

### HTTP Request
`POST http://www.seabookings.com/api/v1/bookings`

### Reservation properties
Parameter | Default | Description
--------- | ------- | -----------
activity_id | - | The id of the activity/experience
slot_id | - | The id of the time slot (time of the booking)
reservation_date | - | The date of booking
customer | - | Customer details
price_fields | - | A list containing the number of people per type of price
terms_of_service | - | A control value that marks that the person has accepted the terms of service. This value must be collected by an opt in control.

### Customer properties
Parameter | Default | Description
--------- | ------- | -----------
name  | - | The name of the customer
email | - | The email of the customer
country_code | - | The country code of the phone number ex: 351
phone_number | - | The phone number of the  customer

### Price fields properties
Parameter | Default | Description
--------- | ------- | -----------
price_id  | - | The id of a price
num_instances | - | The number of times a customer selected that price.

## Retrieve Booking

```shell
curl -X GET \
  'http://www.sb.com:3000/api/v1/bookings/retrieve?pnr=DZR5RN&date=2018-07-28' \
  -H 'Authorization: Bearer dev_token' \
  -H 'Cache-Control: no-cache' \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: c20a39b2-2b40-4bc0-abd0-0176380263af' \
  -H 'Referer: www.seabookings.com' \
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

xhr.open("GET", "http://www.sb.com:3000/api/v1/bookings/retrieve?pnr=DZR5RN&date=2018-07-28");
xhr.setRequestHeader("User-Agent", "SBPORTAL");
xhr.setRequestHeader("Referer", "www.seabookings.com");
xhr.setRequestHeader("Content-Type", "application/json");
xhr.setRequestHeader("Authorization", "Bearer dev_token");
xhr.setRequestHeader("Cache-Control", "no-cache");
xhr.setRequestHeader("Postman-Token", "6b4009f4-95cf-45c9-99d0-4d96c5948464");

xhr.send(data);
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": "18674",
        "type": "booking",
        "attributes": {
            "reservation_date": "2018-07-28",
            "pnr": "DZR5RN",
            "created_at": "2018-07-27T17:28:25.676Z",
            "aggregated_total_cents": 1000,
            "price_total_cents": 1000,
            "application_fee_cents": 200,
            "status": "pending",
            "payment_status": "pending",
            "via": "web_public",
            "customer_note": null,
            "deposit_cents": 1000,
            "price_fields": [
                {
                    "price_id": 42,
                    "num_instances": 1,
                    "label": "Adultos"
                }
            ]
        },
        "relationships": {
            "slot": {
                "data": {
                    "id": "5941",
                    "type": "slot"
                }
            },
            "customer": {
                "data": {
                    "id": "13566",
                    "type": "customer"
                }
            }
        }
    },
    "included": [
        {
            "id": "13566",
            "type": "customer",
            "attributes": {
                "name": "Test User",
                "email": "test@domain.com",
                "country_code": "351",
                "phone_number": "967111111"
            }
        },
        {
            "id": "5941",
            "type": "slot",
            "attributes": {
                "id": 5941,
                "start_at": "2018-07-28",
                "finish_at": "2018-07-28",
                "start_time": "2000-01-01T09:01:00.000Z",
                "finish_time": "2000-01-01T12:00:00.000Z",
                "capacity": 12,
                "cutoff_minutes": 15,
                "deleted_at": null,
                "created_at": "2018-07-28T12:28:05.643Z",
                "updated_at": "2018-07-28T12:28:05.650Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "42",
                            "type": "price"
                        }
                    ]
                }
            }
        }
    ]
}
```

### Query Parameters
Both query parameters are mandatory!

Parameter | Default | Description
--------- | ------- | -----------
date | - | Date of the booking
pnr  | - | Booking unique reference number

## Charge Booking

This endpoint creates a charge for the specified booking.
Bear in mind that the booking status might depend on the policies of the activity.
If the activity requires a manual confirmation from the operator, the status of the booking will be `waiting_for_confirmation` . If the activity has a policy of instant confirmation, the status of the booking will be `booked`.
After a successful charge, the _payment status_ of a booking will always be `confirmed`.

```shell
curl -X POST \
  http://www.sb.com:3000/api/v1/bookings/18677/charge \
  -H 'Authorization: Bearer dev_token' \
  -H 'Cache-Control: no-cache' \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: d9e04202-5c5c-4752-b2ac-aeb0d9e24f56' \
  -d '{
  "payment_gateway": "stripe",
  "token": "tok_visa_debit"
}'
```

```javascript
var data = JSON.stringify({
  "payment_gateway": "stripe",
  "token": "tok_visa_debit"
});

var xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === 4) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "http://www.sb.com:3000/api/v1/bookings/18677/charge");
xhr.setRequestHeader("Content-Type", "application/json");
xhr.setRequestHeader("Authorization", "Bearer dev_token");
xhr.setRequestHeader("Cache-Control", "no-cache");
xhr.setRequestHeader("Postman-Token", "40e2272b-79c2-468f-ad53-930e42463186");

xhr.send(data);
```

> The above command returns JSON structured like this:

```json
{
    "data": {
        "id": "18677",
        "type": "booking",
        "attributes": {
            "reservation_date": "2018-08-02",
            "pnr": "ZNTFVY",
            "created_at": "2018-07-31T09:13:38.644Z",
            "aggregated_total_cents": 1000,
            "price_total_cents": 1000,
            "application_fee_cents": 200,
            "status": "booked",
            "payment_status": "confirmed",
            "via": "web_public",
            "customer_note": null,
            "deposit_cents": 1000,
            "price_fields": [
                {
                    "price_id": 42,
                    "num_instances": 1,
                    "label": "Adultos"
                }
            ]
        },
        "relationships": {
            "slot": {
                "data": {
                    "id": "5942",
                    "type": "slot"
                }
            },
            "customer": {
                "data": {
                    "id": "13569",
                    "type": "customer"
                }
            }
        }
    },
    "included": [
        {
            "id": "13569",
            "type": "customer",
            "attributes": {
                "name": "Test User",
                "email": "test@domain.com",
                "country_code": "351",
                "phone_number": "967111111"
            }
        },
        {
            "id": "5942",
            "type": "slot",
            "attributes": {
                "id": 5942,
                "start_at": "2018-08-01",
                "finish_at": "2018-12-31",
                "start_time": "2000-01-01T09:00:00.000Z",
                "finish_time": "2000-01-01T12:00:00.000Z",
                "capacity": 10,
                "cutoff_minutes": 1440,
                "deleted_at": null,
                "created_at": "2018-07-31T09:08:47.471Z",
                "updated_at": "2018-07-31T09:48:01.260Z"
            },
            "relationships": {
                "prices": {
                    "data": [
                        {
                            "id": "42",
                            "type": "price"
                        },
                        {
                            "id": "14",
                            "type": "price"
                        },
                        {
                            "id": "236",
                            "type": "price"
                        },
                        {
                            "id": "86",
                            "type": "price"
                        },
                        {
                            "id": "400",
                            "type": "price"
                        },
                        {
                            "id": "224",
                            "type": "price"
                        },
                        {
                            "id": "62",
                            "type": "price"
                        },
                        {
                            "id": "401",
                            "type": "price"
                        },
                        {
                            "id": "801",
                            "type": "price"
                        },
                        {
                            "id": "1598",
                            "type": "price"
                        },
                        {
                            "id": "1599",
                            "type": "price"
                        },
                        {
                            "id": "1600",
                            "type": "price"
                        },
                        {
                            "id": "1601",
                            "type": "price"
                        },
                        {
                            "id": "1602",
                            "type": "price"
                        }
                    ]
                }
            }
        }
    ]
}
```

### HTTP Request
`POST http://www.seabookings.com/api/v1/bookings/:booking_id/charge`

### Charge properties
Parameter | Default | Description
--------- | ------- | -----------
payment_gateway: | - | A Gateway identifier: "stripe" or "paypal"
booking_id | - | The booking_id as a url parameter
token | - | The Token/Source obtained via client side from the payment gateway