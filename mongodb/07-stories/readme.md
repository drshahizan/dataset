<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Stories Dataset

The "stories.json" file contains information about a specific story.

## Data Dictionary

| Field Name    | Data Type     | Description                                                                                          |
|---------------|---------------|------------------------------------------------------------------------------------------------------|
| _id           | ObjectId      | Unique identifier for the story                                                                       |
| href          | String        | URL of the story on the Digg website                                                                  |
| title         | String        | Title of the story                                                                                   |
| comments      | Integer       | Number of comments on the story                                                                       |
| container     | Object        | Information about the container or category of the story                                              |
| submit_date   | Integer       | Date and time when the story was submitted (Unix timestamp)                                           |
| topic         | Object        | Information about the topic of the story                                                              |
| promote_date  | Integer       | Date and time when the story was promoted (Unix timestamp)                                            |
| id            | String        | Unique identifier of the story                                                                        |
| media         | String        | Type of media associated with the story                                                               |
| diggs         | Integer       | Number of diggs (votes) received by the story                                                         |
| description   | String        | Brief description of the story                                                                        |
| link          | String        | URL of the article providing more details about the story                                             |
| user          | Object        | Information about the user who submitted the story                                                    |
| status        | String        | Status of the story                                                                                  |
| shorturl      | Array of Objects | Information about the short URL of the story, including the short URL and the view count             |

## Sample Document

```json
{
  "_id": {
    "$oid": "4ba267dc238d3ba3ca000001"
  },
  "href": "http://digg.com/people/Jedi_believer_who_refused_to_remove_hood_gets_an_apology",
  "title": "'Jedi' believer who refused to remove hood gets an apology!",
  "comments": {
    "$numberInt": "153"
  },
  "container": {
    "name": "Offbeat",
    "short_name": "offbeat"
  },
  "submit_date": {
    "$numberInt": "1268771801"
  },
  "topic": {
    "name": "People",
    "short_name": "people"
  },
  "promote_date": {
    "$numberInt": "1268915964"
  },
  "id": "19970068",
  "media": "news",
  "diggs": {
    "$numberInt": "404"
  },
  "description": "Chris Jarvis is a member of the International Church of Jediism - based on the famous Star Wars films - whose doctrine states followers can wear hoods.",
  "link": "http://www.dailymail.co.uk/news/article-1258365/Jedi-believer-wins-apology-Jobcentre-kicked-wearing-hood.html",
  "user": {
    "name": "babychen",
    "registered": {
      "$numberInt": "1141570067"
    },
    "fullname": "Babychen Mathew",
    "icon": "http://digg.com/users/babychen/l.png",
    "profileviews": {
      "$numberInt": "24749"
    }
  },
  "status": "popular",
  "shorturl": [
    {
      "short_url": "http://digg.com/d31Ln7s",
      "view_count": {
        "$numberInt": "3682"
      }
    }
  ]
}

```

| Download <img alt="activity status" height="24" src="../../images/download.png" />|
|:---:|
| <a href="stories.json" ><img src="../../images/dataset.png" ></a>|


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


