<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Dataset: sales.json

The `sample_supplies` database contains data from a mock office supply company. The company tracks customer information and sales data, and has several store locations throughout the world.

To learn how to load the sample data provided by Atlas into your cluster, see [Load Sample Data](#load-sample-data).

## Collections

This database contains a single collection called `sales`.

Each document in the `sample_supplies.sales` collection represents a single sale from a store run by the supply company. Each document contains the items purchased, information on the customer who made the purchase, and several other details regarding the sale.

## Indexes

The `sample_supplies.sales` collection contains the following indexes:

| Name  | Index              | Description                             |
|-------|--------------------|-----------------------------------------|
| _id_  | { "_id": 1 }       | Primary key index on the `_id` field.    |

## Sample Document (json file)

```json
{
  "_id": {
    "$oid": "5bd761dcae323e45a93ccfe8"
  },
  "saleDate": {
    "$date": {
      "$numberLong": "1427144809506"
    }
  },
  "items": [
    {
      "name": "notepad",
      "tags": [
        "office",
        "writing",
        "school"
      ],
      "price": {
        "$numberDecimal": "35.29"
      },
      "quantity": {
        "$numberInt": "2"
      }
    },
    {
      "name": "pens",
      "tags": [
        "writing",
        "office",
        "school",
        "stationary"
      ],
      "price": {
        "$numberDecimal": "56.12"
      },
      "quantity": {
        "$numberInt": "5"
      }
    },
    {
      "name": "envelopes",
      "tags": [
        "stationary",
        "office",
        "general"
      ],
      "price": {
        "$numberDecimal": "19.95"
      },
      "quantity": {
        "$numberInt": "8"
      }
    },
    {
      "name": "binder",
      "tags": [
        "school",
        "general",
        "organization"
      ],
      "price": {
        "$numberDecimal": "14.16"
      },
      "quantity": {
        "$numberInt": "3"
      }
    }
  ],
  "storeLocation": "Denver",
  "customer": {
    "gender": "M",
    "age": {
      "$numberInt": "42"
    },
    "email": "cauho@witwuta.sv",
    "satisfaction": {
      "$numberInt": "4"
    }
  },
  "couponUsed": true,
  "purchaseMethod": "Online"
}
```

## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


