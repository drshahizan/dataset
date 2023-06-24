<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Airbnb Listings Dataset

The airbnb database is a compilation of vacation home listings and reviews available on Inside AirBnB. This database contains a single collection called `listingsAndReviews`. The `listingsAndReviews` collection contains documents that represent the vacation home listing details and reviews of customers about the listing. These documents reflect a randomized subset of the original publicly available source, from several different cities around the globe.

## Data Dictionary

| Field                    | Type           | Description |
|--------------------------|----------------|----------------------------------------------------------------------------------------------------------|
| `_id` | String         | Unique identifier for the listing                                                                         |
| `listing_url` | String         | URL of the listing on Airbnb                                                                              |
| `name` | String         | Name of the listing                                                                                       |
| `summary` | String         | Summary description of the listing                                                                         |
| `interaction` | String         | Information about interaction with the host                                                               |
| `house_rules` | String         | House rules for guests                                                                                    |
| `property_type` | String         | Type of property (e.g., house, apartment, etc.)                                                           |
| `room_type` | String         | Type of room (e.g., entire home/apt, private room, etc.)                                                  |
| `bed_type` | String         | Type of bed (e.g., real bed, sofa bed, etc.)                                                              |
| `minimum_nights` | String         | Minimum number of nights for a booking                                                                     |
| `maximum_nights` | String         | Maximum number of nights for a booking                                                                     |
| `cancellation_policy` | String         | Cancellation policy for the listing |
| `last_scraped` | Date           | Date when the listing was last scraped                                                                     |
|` calendar_last_scraped` | Date           | Date when the calendar was last scraped |
| `first_review` | Date           | Date of the first review for the listing                                                                   |
| `last_review` | Date           | Date of the most recent review for the listing                                                             |
| `accommodates` | Integer        | Number of guests the listing can accommodate                                                               |
| `bedrooms` | Integer        | Number of bedrooms                                                                                        |
| `beds` | Integer        | Number of beds                                                                                            |
| `number_of_reviews` | Integer        | Total number of reviews for the listing |
| `bathrooms` | Decimal        | Number of bathrooms                                                                                       |
| `amenities` | Array of strings | List of amenities provided in the listing                                                                  |
| `price` | Decimal        | Price per night                                                                                           |
| `security_deposit` | Decimal        | Security deposit amount                                                                                    |
| `cleaning_fee` | Decimal        | Cleaning fee amount                                                                                        |
| `extra_people` | Decimal        | Additional fee for extra guests                                                                            |
| `guests_included` | Decimal        | Number of guests included in the base price                                                                |
| `images` | Object         | URLs of images associated with the listing                                                                 |
| `host` | Object         | Information about the host                                                                                 |
| `address` | Object         | Address information for the listing                                                                        |
| `availability` | Object         | Availability information for the listing                                                                   |
| `review_scores` | Object         | Ratings and scores for the listing                                                                         |
| `reviews` | Array of objects | List of reviews for the listing                                                                            |

## Sample Document

```json
{
  "_id": "10006546",
  "listing_url": "https://www.airbnb.com/rooms/10006546",
  "name": "Ribeira Charming Duplex",
  "summary": "Fantastic duplex apartment with three bedrooms, located in the historic area of Porto, Ribeira (Cube)...",
  "interaction": "Cot - 10 € / night Dog - € 7,5 / night",
  "house_rules": "Make the house your home...",
  "property_type": "House",
  "room_type": "Entire home/apt",
  "bed_type": "Real Bed",
  "minimum_nights": "2",
  "maximum_nights": "30",
  "cancellation_policy": "moderate",
  "last_scraped": {
    "$date": {
      "$numberLong": "1550293200000"
    }
  },
  "calendar_last_scraped": {
    "$date": {
      "$numberLong": "1550293200000"
    }
  },
  "first_review": {
    "$date": {
      "$numberLong": "1451797200000"
    }
  },
  "last_review": {
    "$date": {
      "$numberLong": "1547960400000"
    }
  },
  "accommodates": {
    "$numberInt": "8"
  },
  "bedrooms": {
    "$numberInt": "3"
  },
  "beds": {
    "$numberInt": "5"
  },
  "number_of_reviews": {
    "$numberInt": "51"
  },
  "bathrooms": {
    "$numberDecimal": "1.0"
  },
  "amenities": [
    "TV",
    "Cable TV",
    "Wifi",
    "Kitchen",
    "Paid parking off premises",
    "Smoking allowed",
    "Pets allowed",
    "Buzzer/wireless intercom",
    "Heating",
    "Family/kid friendly",
    "Washer",
    "First aid kit",
    "Fire extinguisher",
    "Essentials",
    "Hangers",
    "Hair dryer",
    "Iron",
    "Pack ’n Play/travel crib",
    "Room-darkening shades",
    "Hot water",
    "Bed linens",
    "Extra pillows and blankets",
    "Microwave",
    "Coffee maker",
    "Refrigerator",
    "Dishwasher",
    "Dishes and silverware",
    "Cooking basics",
    "Oven",
    "Stove",
    "Cleaning before checkout",
    "Waterfront"
  ],
  "price": {
    "$numberDecimal": "80.00"
  },
  "security_deposit": {
    "$numberDecimal": "200.00"
  },
  "cleaning_fee": {
    "$numberDecimal": "35.00"
  },
  "extra_people": {
    "$numberDecimal": "15.00"
  },
  "guests_included": {
    "$numberDecimal": "6"
  },
  "images": {
    "thumbnail_url": "",
    "medium_url": "",
    "picture_url": "https://a0.muscache.com/im/pictures/e83e702f-ef49-40fb-8fa0-6512d7e26e9b.jpg?aki_policy=large",
    "xl_picture_url": ""
  },
  "host": {
    "host_id": "51399391",
    "host_url": "https://www.airbnb.com/users/show/51399391",
    "host_name": "Ana&Gonçalo",
    "host_location": "Porto, Porto District, Portugal",
    "host_about": "Gostamos de passear, de viajar, de conhecer pessoas e locais novos, gostamos de desporto e animais! Vivemos na cidade mais linda do mundo!!!",
    "host_response_time": "within an hour",
    "host_thumbnail_url": "https://a0.muscache.com/im/pictures/fab79f25-2e10-4f0f-9711-663cb69dc7d8.jpg?aki_policy=profile_small",
    "host_picture_url": "https://a0.muscache.com/im/pictures/fab79f25-2e10-4f0f-9711-663cb69dc7d8.jpg?aki_policy=profile_x_medium",
    "host_neighbourhood": "",
    "host_response_rate": {
      "$numberInt": "100"
    },
    "host_is_superhost": false,
    "host_has_profile_pic": true,
    "host_identity_verified": true,
    "host_listings_count": {
      "$numberInt": "3"
    },
    "host_total_listings_count": {
      "$numberInt": "3"
    },
    "host_verifications": [
      "email",
      "phone",
      "reviews",
      "jumio",
      "offline_government_id",
      "government_id"
    ]
  },
  "address": {
    "street": "Porto, Porto, Portugal",
    "suburb": "",
    "government_area": "Cedofeita, Ildefonso, Sé, Miragaia, Nicolau, Vitória",
    "market": "Porto",
    "country": "Portugal",
    "country_code": "PT",
    "location": {
      "type": "Point",
      "coordinates": [
        {
          "$numberDouble": "-8.61308"
        },
        {
          "$numberDouble": "41.1413"
        }
      ],
      "is_location_exact": false
    }
  },
  "availability": {
    "availability_30": {
      "$numberInt": "28"
    },
    "availability_60": {
      "$numberInt": "47"
    },
    "availability_90": {
      "$numberInt": "74"
    },
    "availability_365": {
      "$numberInt": "239"
    }
  },
  "review_scores": {
    "review_scores_accuracy": {
      "$numberInt": "9"
    },
    "review_scores_cleanliness": {
      "$numberInt": "9"
    },
    "review_scores_checkin": {
      "$numberInt": "10"
    },
    "review_scores_communication": {
      "$numberInt": "10"
    },
    "review_scores_location": {
      "$numberInt": "10"
    },
    "review_scores_value": {
      "$numberInt": "9"
    },
    "review_scores_rating": {
      "$numberInt": "89"
    }
  },
  "reviews": [
    {
      "_id": "362865132",
      "date": {
        "$date": {
          "$numberLong": "1545886800000"
        }
      },
      "listing_id": "10006546",
      "reviewer_id": "208880077",
      "reviewer_name": "Thomas",
      "comments": "Very helpful hosts. Cooked traditional..."
    },
    {
      "_id": "364728730",
      "date": {
        "$date": {
          "$numberLong": "1546232400000"
        }
      },
      "listing_id": "10006546",
      "reviewer_id": "91827533",
      "reviewer_name": "Mr",
      "comments": "Ana & Goncalo were great on communication..."
    },
    {
      "_id": "403055315",
      "date": {
        "$date": {
          "$numberLong": "1547960400000"
        }
      },
      "listing_id": "10006546",
      "reviewer_id": "15138940",
      "reviewer_name": "Milo",
      "comments": "The house was extremely well located..."
    }
  ]
}
```

| Download <img alt="activity status" height="24" src="../../images/download.png" />|
|:---:|
| <a href="listingsAndReviews.json" ><img src="../../images/dataset.png" ></a>|

## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


