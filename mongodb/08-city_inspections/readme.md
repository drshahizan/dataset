<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# City Inspections Dataset
The City Inspections Dataset provides information about inspections conducted in a city. 

## Data Dictionary

| No | Field                 | Type     | Description                                       |
|----|-----------------------|----------|---------------------------------------------------|
| 1  | \_id                  | Object   | Unique identifier for the inspection record        |
| 2  | id                    | String   | Identifier for the inspection                     |
| 3  | certificate_number    | Number   | Certificate number associated with the business    |
| 4  | business_name         | String   | Name of the inspected business                    |
| 5  | date                  | String   | Date of the inspection                            |
| 6  | result                | String   | Result of the inspection                           |
| 7  | sector                | String   | Sector or category of the business                |
| 8  | address               | Object   | Address details of the business                    |
| 8a | - city                | String   | City where the business is located                |
| 8b | - zip                 | Number   | ZIP code of the business                          |
| 8c | - street              | String   | Street name of the business                       |
| 8d | - number              | Number   | Street number of the business                     |

## Sample Document

```json
{
  "_id": { "$oid": "56d61033a378eccde8a8354f" },
  "id": "10021-2015-ENFO",
  "certificate_number": 9278806,
  "business_name": "ATLIXCO DELI GROCERY INC.",
  "date": "Feb 20 2015",
  "result": "No Violation Issued",
  "sector": "Cigarette Retail Dealer - 127",
  "address": {
    "city": "RIDGEWOOD",
    "zip": 11385,
    "street": "MENAHAN ST",
    "number": 1712
  }
}
```

| Download <img alt="activity status" height="24" src="../../images/download.png" />|
|:---:|
| <a href="city_inspections.json" ><img src="../../images/dataset.png" ></a>|


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


