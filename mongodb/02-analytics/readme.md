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
| Accounts        | This collection contains account details for users. Each document contains an account id, a limit and the products that a customer has purchased. |
| Customers       | This collection contains customers details including what accounts they hold users. Each document contains username, name, address, birth date, email address, a list of the accounts held, and details on the tiers and related benefits they are entitled to. |
| Transactions    | This collection contains transactions details for users. Each document contains an account id, a count of how many transactions are in this set, the start and end dates for transactions covered by this document, and a list of sub documents. Each sub document represents a single transaction and the related information for that transaction. |

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

## Sample Document
Sure! Here's the JSON code in Markdown format:

**Comments**
```json
{
  "_id": {
    "$oid": "5a9427648b0beebeb69579cc"
  },
  "name": "Andrea Le",
  "email": "andrea_le@fakegmail.com",
  "movie_id": {
    "$oid": "573a1390f29313caabcd418c"
  },
  "text": "Rem officiis eaque repellendus amet eos doloribus. Porro dolor voluptatum voluptates neque culpa molestias. Voluptate unde nulla temporibus ullam.",
  "date": {
    "$date": {
      "$numberLong": "1332804016000"
    }
  }
}
```

**Customers**
```json
{
  "_id": {
    "$oid": "5ca4bbcea2dd94ee58162a68"
  },
  "username": "fmiller",
  "name": "Elizabeth Ray",
  "address": "9286 Bethany Glens\nVasqueztown, CO 22939",
  "birthdate": {
    "$date": {
      "$numberLong": "226117231000"
    }
  },
  "email": "arroyocolton@gmail.com",
  "active": true,
  "accounts": [
    {
      "$numberInt": "371138"
    },
    {
      "$numberInt": "324287"
    },
    {
      "$numberInt": "276528"
    },
    {
      "$numberInt": "332179"
    },
    {
      "$numberInt": "422649"
    },
    {
      "$numberInt": "387979"
    }
  ],
  "tier_and_details": {
    "0df078f33aa74a2e9696e0520c1a828a": {
      "tier": "Bronze",
      "id": "0df078f33aa74a2e9696e0520c1a828a",
      "active": true,
      "benefits": [
        "sports tickets"
      ]
    },
    "699456451cc24f028d2aa99d7534c219": {
      "tier": "Bronze",
      "benefits": [
        "24 hour dedicated line",
        "concierge services"
      ],
      "active": true,
      "id": "699456451cc24f028d2aa99d7534c219"
    }
  }
}
```

**Transactions**
```json
{
  "_id": { "$oid": "5ca4bbc1a2dd94ee58161cb1" },
  "account_id": { "$numberInt": "443178" },
  "transaction_count": { "$numberInt": "66" },
  "bucket_start_date": { "$date": { "$numberLong": "-28598400000" } },
  "bucket_end_date": { "$date": { "$numberLong": "1483401600000" } },
  "transactions": [
    {
      "date": { "$date": { "$numberLong": "1063065600000" } },
      "amount": { "$numberInt": "7514" },
      "transaction_code": "buy",
      "symbol": "adbe",
      "price": "19.1072802650074180519368383102118968963623046875",
      "total": "143572.1039112657392422534031"
    },
    {
      "date": { "$date": { "$numberLong": "1465862400000" } },
      "amount": { "$numberInt": "9240" },
      "transaction_code": "buy",
      "symbol": "team",
      "price": "24.1525632387771480580340721644461154937744140625",
      "total": "223169.6843263008480562348268"
    },
    {
      "date": { "$date": { "$numberLong": "1038960000000" } },
      "amount": { "$numberInt": "2824" },
      "transaction_code": "buy",
      "symbol": "msft",
      "price": "21.046193953245431629284212249331176280975341796875",
      "total": "59434.45172396509892109861539"
    },
    {
      "date": { "$date": { "$numberLong": "1405296000000" } },
      "amount": { "$numberInt": "7418" },
      "transaction_code": "sell",
      "symbol": "sap",
      "price": "76.38514540536692720706923864781856536865234375",
      "total": "566625.0086170118660220396123"
    },
    {
      "date": { "$date": { "$numberLong": "1319760000000" } },
      "amount": { "$numberInt": "5638" },
      "transaction_code": "buy",
      "symbol": "adbe",
      "price": "28.365657608641175357888641883619129657745361328125",
      "total": "159925.5775975189466677761629"
    },
    {
      "date": { "$date": { "$numberLong": "1292803200000" } },
      "amount": { "$numberInt": "6774" },
      "transaction_code": "sell",
      "symbol": "sap",
      "price": "45.3237971108758159743956639431416988372802734375",
      "total": "307023.4016290727774105562276"
    },
    {
      "date": { "$date": { "$numberLong": "1445990400000" } },
      "amount": { "$numberInt": "7251" },
      "transaction_code": "sell",
      "symbol": "nflx",
      "price": "102.936674838205050264150",
      "total": "143572.1039112657392422534031"
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


