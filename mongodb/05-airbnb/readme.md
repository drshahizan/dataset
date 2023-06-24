<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Mflix Dataset

The database contains data on movies and movie theaters. The database also contains collections for certain metadata, including users and comments on specific movies.

| Collection Name | Description                                |
|-----------------|--------------------------------------------|
| Comments | This collection contains comments associated with specific movies. Each document contains the comment text, the user who submitted it, and the movie the comment applies to. |
| Movies | This collection contains details on movies. Each document contains a single movie, and information such as its title, release year, and cast. |
| Theaters | This collection contains movie theater locations. Each document contains a single movie theater and its location in both string and GeoJSON forms.|
|Users| This collection contains information on mflix users. Each document contains a single user, and their name, email, and password.|

## Data Dictionary

**Comments**

| Field         | Type         | Description                                 |
|---------------|--------------|---------------------------------------------|
| `_id`         | ObjectId     | Unique identifier for the comment.           |
| `name`        | String       | Name of the commenter.                       |
| `email`       | String       | Email address of the commenter.              |
| `movie_id`    | ObjectId     | Unique identifier of the associated movie.   |
| `text`        | String       | The actual comment text.                     |
| `date`        | Date         | Date and time of the comment.                |

**Movies**

| Field                | Type          | Description                                                       |
|----------------------|---------------|-------------------------------------------------------------------|
| `_id`                | ObjectId      | Unique identifier for the movie.                                   |
| `plot`               | String        | Brief description or summary of the movie.                         |
| `genres`             | Array[String] | Array of genres associated with the movie.                         |
| `runtime`            | NumberInt     | Duration of the movie in minutes.                                  |
| `cast`               | Array[String] | Array of actors appearing in the movie.                            |
| `num_mflix_comments` | NumberInt     | Number of comments/reviews for the movie.                          |
| `title`              | String        | Title of the movie.                                                |
| `fullplot`           | String        | Detailed description or plot summary of the movie.                 |
| `countries`          | Array[String] | Array of countries where the movie was produced.                   |
| `released`           | Date          | Date of movie release.                                             |
| `directors`          | Array[String] | Array of directors of the movie.                                   |
| `rated`              | String        | Rating of the movie (e.g., "UNRATED", "PG-13").                     |
| `awards`             | Object        | Information about the awards won by the movie.                     |
| `lastupdated`        | String        | Date and time of the last update to the movie information.          |
| `year`               | NumberInt     | Year of the movie release.                                         |
| `imdb`               | Object        | IMDb-related information, including rating, votes, and ID.          |
| `type`               | String        | Type of content (e.g., "movie", "series").                          |
| `tomatoes`           | Object        | Information related to the movie's rating on Rotten Tomatoes.       |

**Theaters**

| Field             | Type                | Description                                             |
|-------------------|---------------------|---------------------------------------------------------|
| `_id`             | ObjectId            | Unique identifier for the theater.                      |
| `theaterId`       | NumberInt           | Identifier for the theater.                             |
| `location`        | Object              | Location information of the theater, including address and geographic coordinates. |

**Users**

| Field         | Type         | Description                                 |
|---------------|--------------|---------------------------------------------|
| `_id`         | ObjectId     | Unique identifier for the user.              |
| `name`        | String       | Name of the user.                            |
| `email`       | String       | Email address of the user.                   |
| `password`    | String       | Encrypted password of the user.              |

## Sample Document

**Comments**
```json
{
  "_id": {"$oid": "5a9427648b0beebeb69579cc"},
  "name": "Andrea Le",
  "email": "andrea_le@fakegmail.com",
  "movie_id": {"$oid": "573a1390f29313caabcd418c"},
  "text": "Rem officiis eaque repellendus amet eos doloribus. Porro dolor voluptatum voluptates neque culpa molestias. Voluptate unde nulla temporibus ullam.",
  "date": {"$date": {"$numberLong": "1332804016000"}}
}
```

**Movies**
```json
{
  "_id": {"$oid": "573a1390f29313caabcd4135"},
  "plot": "Three men hammer on an anvil and pass a bottle of beer around.",
  "genres": ["Short"],
  "runtime": {"$numberInt": "1"},
  "cast": ["Charles Kayser", "John Ott"],
  "num_mflix_comments": {"$numberInt": "1"},
  "title": "Blacksmith Scene",
  "fullplot": "A stationary camera looks at a large anvil with a blacksmith behind it and one on either side. The smith in the middle draws a heated metal rod from the fire, places it on the anvil, and all three begin a rhythmic hammering. After several blows, the metal goes back in the fire. One smith pulls out a bottle of beer, and they each take a swig. Then, out comes the glowing metal and the hammering resumes.",
  "countries": ["USA"],
  "released": {"$date": {"$numberLong": "-2418768000000"}},
  "directors": ["William K.L. Dickson"],
  "rated": "UNRATED",
  "awards": {"wins": {"$numberInt": "1"}, "nominations": {"$numberInt": "0"}, "text": "1 win."},
  "lastupdated": "2015-08-26 00:03:50.133000000",
  "year": {"$numberInt": "1893"},
  "imdb": {"rating": {"$numberDouble": "6.2"}, "votes": {"$numberInt": "1189"}, "id": {"$numberInt": "5"}},
  "type": "movie",
  "tomatoes": {
    "viewer": {"rating": {"$numberInt": "3"}, "numReviews": {"$numberInt": "184"}, "meter": {"$numberInt": "32"}},
    "lastUpdated": {"$date": {"$numberLong": "1435516449000"}}
  }
}
```

**Theaters**
```json
{
  "_id": {"$oid": "59a47286cfa9a3a73e51e72c"},
  "theaterId": {"$numberInt": "1000"},
  "location": {
    "address": {
      "street1": "340 W Market",
      "city": "Bloomington",
      "state": "MN",
      "zipcode": "55425"
    },
    "geo": {
      "type": "Point",
      "coordinates": [{"$numberDouble": "-93.24565"}, {"$numberDouble": "44.85466"}]
    }
  }
}
```

**Users**
```json
{
  "_id": {"$oid": "59b99db4cfa9a34dcd7885b6"},
  "name": "Ned Stark",
  "email": "sean_bean@gameofthron.es",
  "password": "$2b$12$UREFwsRUoyF0CRqGNK0LzO0HM/jLhgUCNNIJ9RJAqMUQ74crlJ1Vu"
}
```

| Download |<img alt="activity status" height="24" src="../../images/download.png" />|
|---|:---:|
| Comments |<a href="comments.json" ><img src="../../images/dataset.png" width="24px" height="24px" ></a>|
| Movies|<a href="movies.json" ><img src="../../images/dataset.png" width="24px" height="24px" ></a>|
| Theaters|<a href="theaters.json" ><img src="../../images/dataset.png" width="24px" height="24px" ></a>|
| Users |<a href="users" ><img src="../../images/dataset.png" width="24px" height="24px" ></a>|


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


