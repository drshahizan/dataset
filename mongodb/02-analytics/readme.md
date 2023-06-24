<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Analytics Dataset

The analytics database contains three collections for a typical finanacial services application. It has customers, accounts, and transactions. 

| Collection Name | Description                                |
|-----------------|--------------------------------------------|
| accounts        | This collection contains account details for users. Each document contains an account id, a limit and the products that a customer has purchased. |
| customers       | This collection contains customers details including what accounts they hold users. Each document contains username, name, address, birth date, email address, a list of the accounts held, and details on the tiers and related benefits they are entitled to. |
| transactions    | This collection contains transactions details for users. Each document contains an account id, a count of how many transactions are in this set, the start and end dates for transactions covered by this document, and a list of sub documents. Each sub document represents a single transaction and the related information for that transaction. |

## Data Dictionary

The dataset consists of three tables: "Accounts," "Customers," and "Transactions." Each table represents a specific aspect of the data and provides valuable information it.

**Accounts**

| Field        | Type       | Description                                          |
|--------------|------------|------------------------------------------------------|
| account_id   | Integer    | The unique identifier for the account.                |
| limit        | Integer    | The account's limit.                                 |
| products     | Array      | A list of products associated with the account.       |


**Customers**

| Field            | Type       | Description                                              |
|------------------|------------|----------------------------------------------------------|
| username         | String     | The username of the customer.                             |
| name             | String     | The name of the customer.                                 |
| address          | String     | The customer's address.                                   |
| birthdate        | Date       | The customer's birthdate in UNIX timestamp format.        |
| email            | String     | The customer's email address.                             |
| accounts         | Array      | A list of account IDs associated with the customer.       |
| tier_and_details | Object     | Additional details about the customer's tier.             |


**Transactions**

| Field              | Type       | Description                                           |
|--------------------|------------|-------------------------------------------------------|
| account_id         | Integer    | The unique identifier for the account associated with the transactions. |
| transaction_count  | Integer    | The number of transactions.                           |
| bucket_start_date  | Date       | The start date of the transaction bucket in UNIX timestamp format. |
| bucket_end_date    | Date       | The end date of the transaction bucket in UNIX timestamp format. |
| transactions       | Array      | A list of individual transaction details.              |

Please note that the data types provided in the table are based on the example data provided in the JSON files.

## Sample Document

**Accounts**
```json
{
  "account_id": 470650,
  "limit": 10000,
  "products": [
    "CurrencyService",
    "Commodity",
    "InvestmentStock"
  ]
}
```

**Customers**
```json
{
 "username": "lejoshua",
 "name": "Michael Johnson",
 "address": "15989 Edward Inlet\nLake Maryton, NC 39545",
 "birthdate": {"$date": 54439275000},
 "email": "courtneypaul@gmail.com",
 "accounts": [
   470650,
   443178
 ],
 "tier_and_details": {
   "b5f19cb532fa436a9be2cf1d7d1cac8a": {
      "tier": "Silver",
      "benefits": [
        "dedicated account representative"
      ],
      "active": true,
      "id": "b5f19cb532fa436a9be2cf1d7d1cac8a"
      }
 }
}
```

**Transactions**
```json
{
  "account_id": 794875,
  "transaction_count": 6,
  "bucket_start_date": {"$date": 693792000000},
  "bucket_end_date": {"$date": 1473120000000},
  "transactions": [
    {
      "date": {"$date": 1325030400000},
      "amount": 1197,
      "transaction_code": "buy",
      "symbol": "nvda",
      "price": "12.7330024299341033611199236474931240081787109375",
      "total": "15241.40390863112172326054861"
    },
    {
       "date": {"$date": 1465776000000},
       "amount": 8797,
       "transaction_code": "buy",
       "symbol": "nvda",
       "price": "46.53873172406391489630550495348870754241943359375",
       "total": "409401.2229765902593427995271"
    },
    {
       "date": {"$date": 1472601600000},
       "amount": 6146,
       "transaction_code": "sell",
       "symbol": "ebay",
       "price": "32.11600884852845894101847079582512378692626953125",
       "total": "197384.9903830559086514995215"
    },
    {
       "date": {"$date": 1101081600000},
       "amount": 253,
       "transaction_code": "buy",
       "symbol": "amzn",
       "price": "37.77441226157566944721111212857067584991455078125",
       "total": "9556.926302178644370144411369"
    },
    {
       "date": {"$date": 1022112000000},
       "amount": 4521,
       "transaction_code": "buy",
       "symbol": "nvda",
       "price": "10.763069758141103449133879621513187885284423828125",
       "total": "48659.83837655592869353426977"
    },
    {
       "date": {"$date": 936144000000},
       "amount": 955,
       "transaction_code": "buy",
       "symbol": "csco",
       "price": "27.992136535152877030441231909207999706268310546875",
       "total": "26732.49039107099756407137647"
    }
  ]
}
```

| Download |<img alt="activity status" height="24" src="../../images/download.png" />|
|---|:---:|
| Accounts |<a href="accounts.json" ><img src="../../images/dataset.png" width="24px" height="24px" ></a>|
| Customers|<a href="customer.json" ><img src="../../images/dataset.png" width="24px" height="24px" ></a>|
| Transactions|<a href="transactions.json" ><img src="../../images/dataset.png" width="24px" height="24px" ></a>|


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


