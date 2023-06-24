<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Supply Store Dataset

This database contains a single collection called `sales`.

Each document in the collection represents a single sale from a store run by the supply company. Each document contains the items purchased, information on the customer who made the purchase, and several other details regarding the sale. It contains information about individual sales transactions, including the items purchased, customer details, store location, coupon usage, and purchase method.

## Data Dictionary

| No. | Field           | Description                                                                                    |
|-----:|-----------------|------------------------------------------------------------------------------------------------|
| 1   | _id             | A unique identifier for the sale document.                                                    |
| 2   | saleDate        | The date and time of the sale.                                                                 |
| 3   | items           | An array of items purchased in the sale.                                                       |
|     | - name          | The name of the item.                                                                         |
|     | - tags          | An array of tags describing the item.                                                          |
|     | - price         | The price of the item.                                                                        |
|     | - quantity      | The quantity of the item purchased.                                                            |
| 4   | storeLocation   | The location of the store where the sale took place.                                           |
| 5   | customer        | Information about the customer who made the purchase.                                          |
|     | - gender        | The gender of the customer.                                                                   |
|     | - age           | The age of the customer.                                                                      |
|     | - email         | The email address of the customer.                                                             |
|     | - satisfaction  | The satisfaction level of the customer.                                                        |
| 6   | couponUsed      | A boolean value indicating whether a coupon was used in the sale.                              |
| 7   | purchaseMethod  | The method of purchase, such as "Online" or "In-store".                                        |

>Please note that the "items" and "customer" fields contain nested attributes represented as sub-tables within the main table.

The dataset provides valuable insights into the sales activities of the office supply company, including the specific items sold, customer demographics, store locations, and sales channels. Analyzing this dataset can help identify popular items, customer preferences, sales trends, and other relevant business insights.

## Sample Document

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
      "name": "printer paper",
      "tags": [
        "office",
        "stationary"
      ],
      "price": {
        "$numberDecimal": "40.01"
      },
      "quantity": {
        "$numberInt": "2"
      }
    },
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
      "name": "backpack",
      "tags": [
        "school",
        "travel",
        "kids"
      ],
      "price": {
        "$numberDecimal": "77.71"
      },
      "quantity": {
        "$numberInt": "2"
      }
    },
    {
      "name": "notepad",
      "tags": [
        "office",
        "writing",
        "school"
      ],
      "price": {
        "$numberDecimal": "18.47"
      },
      "quantity": {
        "$numberInt": "2"
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
      "name": "envelopes",
      "tags": [
        "stationary",
        "office",
        "general"
      ],
      "price": {
        "$numberDecimal": "8.08"
      },
      "quantity": {
        "$numberInt": "3"
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

| <img alt="activity status" align="right" height="24" src="../../images/download.png" /> ✅ Download |
|:---:|
|  <a href="sales.json" ><img src="../../images/dataset.png"></a> |


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


