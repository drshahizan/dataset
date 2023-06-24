<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Companies Dataset

This collection contains information on companies listed on Crunchbase. It has a variety of information such as the company website and/or blog websites about the company, funding rounds, and known individuals associated with the company.

## Data Dictionary

| Field                  | Type           | Description |
|------------------------|----------------|--------------------------------------------------------------------------------------------------------------------|
| `_id` | Object         | Unique identifier for the company                                                                                    |
| `acquisition` | Null           | Information about the company's acquisition |
| `acquisitions` | Array          | List of acquisitions made by the company |
| `alias_list` | Null           | List of alternative names or aliases for the company |
| `blog_feed_url` | String         | URL of the company's blog feed |
| `blog_url` | String         | URL of the company's blog |
| `category_code` | String         | Category code representing the company's industry or sector |
| `competitions` | Array          | List of competitors for the company |
| `created_at` | String         | Date and time when the company's information was created |
| `crunchbase_url` | String         | URL of the company's Crunchbase profile |
| `deadpooled_day` | Null           | Day when the company was declared dead or no longer operational |
| `deadpooled_month` | Null           | Month when the company was declared dead or no longer operational |
| `deadpooled_url` | Null           | URL providing additional information about the company's deadpooled status |
| `deadpooled_year` | Null           | Year when the company was declared dead or no longer operational |
| `description` | Null           | Description of the company |
| `email_address` | String         | Email address of the company |
| `external_links` | Array          | List of external links related to the company |
| `founded_day` | Integer        | Day when the company was founded |
| `founded_month` | Integer        | Month when the company was founded |
| `founded_year` | Integer        | Year when the company was founded |
| `funding_rounds` | Array          | List of funding rounds for the company |
| `homepage_url` | String         | URL of the company's homepage |
| `image` | Object         | Information about the company's image or logo |
| `investments` | Array          | List of investments made by the company |
| `ipo` | Null           | Information about the company's initial public offering (IPO) |
| `milestones` | Array          | List of milestones achieved by the company |
| `name` | String         | Name of the company |
| `number_of_employees` | Integer        | Number of employees at the company |
| `offices` | Array          | List of offices or locations associated with the company |
| `overview` | String         | Overview or description of the company |
| `partners` | Array          | List of partners or affiliations of the company |
| `permalink` | String         | Unique permalink or URL slug for the company |
| `phone_number` | String         | Phone number of the company |
| `products` | Array          | List of products offered by the company |
| `providerships` | Array          | List of providerships or partnerships of the company |
| `relationships` | Array          | List of relationships or roles of individuals associated with the company |
| `screenshots` | Array          | List of screenshots or images associated with the company |
| `tag_list` | Null           | List of tags or keywords associated with the company |
| `total_money_raised` | String         | Total amount of money raised by the company |
| `twitter_username` | Null           | Twitter username of the company |
| `updated_at` | String         | Date and time when the company's information was last updated |
| `video_embeds` | Array          | List of video embeds associated with the company |

## Sample Document

```json
{
  "_id": {
      "$oid": "52cdef7c4bab8bd675298291"
  },
  "acquisition": null,
  "acquisitions": [],
  "alias_list": null,
  "blog_feed_url": "http://mobiance.wordpress.com/feed/",
  "blog_url": "http://mobiance.wordpress.com/",
  "category_code": "web",
  "competitions": [],
  "created_at": "Tue Feb 12 17:31:58 UTC 2008",
  "crunchbase_url": "http://www.crunchbase.com/company/mobiance",
  "deadpooled_day": null,
  "deadpooled_month": null,
  "deadpooled_url": null,
  "deadpooled_year": null,
  "description": null,
  "email_address": "info@mobiance.com",
  "external_links": [],
  "founded_day": {
      "$numberInt": "1"
  },
  "founded_month": {
      "$numberInt": "10"
  },
  "founded_year": {
      "$numberInt": "2004"
  },
  "funding_rounds": [],
  "homepage_url": "http://www.mobiance.com",
  "image": {
      "attribution": null,
      "available_sizes": [
          [
              [
                  {
                      "$numberInt": "150"
                  },
                  {
                      "$numberInt": "43"
                  }
              ],
              "assets/images/resized/0001/1859/11859v1-max-150x150.png"
          ],
          [
              [
                  {
                      "$numberInt": "208"
                  },
                  {
                      "$numberInt": "60"
                  }
              ],
              "assets/images/resized/0001/1859/11859v1-max-250x250.png"
          ],
          [
              [
                  {
                      "$numberInt": "208"
                  },
                  {
                      "$numberInt": "60"
                  }
              ],
              "assets/images/resized/0001/1859/11859v1-max-450x450.png"
          ]
      ]
  },
  "investments": [],
  "ipo": null,
  "milestones": [],
  "name": "Mobiance",
  "number_of_employees": {
      "$numberInt": "5"
  },
  "offices": [
      {
          "address1": "BC-3, Atrium Business Center,",
          "address2": "Coles Road, Frazer Town,",
          "city": "Bangalore",
          "country_code": "IND",
          "description": null,
          "latitude": null,
          "longitude": null,
          "state_code": null,
          "zip_code": "560005"
      }
  ],
  "overview": "<p>Mobiance provides the technology to track cell phones ...",
  "partners": [],
  "permalink": "mobiance",
  "phone_number": "+91-80- 41264756",
  "products": [],
  "providerships": [],
  "relationships": [
      {
          "is_past": true,
          "person": {
              "first_name": "Ritesh",
              "last_name": "Ambastha",
              "permalink": "ritesh-ambastha"
          },
          "title": "Product Manager"
      }
  ],
  "screenshots": [],
  "tag_list": null,
  "total_money_raised": "$0",
  "twitter_username": null,
  "updated_at": "Thu Dec 01 07:37:10 UTC 2011",
  "video_embeds": []
}
```

| Download <img alt="activity status" height="24" src="../../images/download.png" />|
|:---:|
| <a href="companies.json" ><img src="../../images/dataset.png" ></a>|


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


