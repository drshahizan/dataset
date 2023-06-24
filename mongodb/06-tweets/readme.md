<a href="https://github.com/drshahizan/dataset/stargazers"><img src="https://img.shields.io/github/stars/drshahizan/dataset" alt="Stars Badge"/></a>
<a href="https://github.com/drshahizan/dataset/network/members"><img src="https://img.shields.io/github/forks/drshahizan/dataset" alt="Forks Badge"/></a>
<a href="https://github.com/drshahizan/dataset/pulls"><img src="https://img.shields.io/github/issues-pr/drshahizan/dataset" alt="Pull Requests Badge"/></a>
<a href="https://github.com/drshahizan/dataset/issues"><img src="https://img.shields.io/github/issues/drshahizan/dataset" alt="Issues Badge"/></a>
<a href="https://github.com/drshahizan/dataset/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/drshahizan/dataset?color=2b9348"></a>
![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan%2Fdataset&labelColor=%23d9e3f0&countColor=%23697689&style=flat)

Don't forget to hit the :star: if you like this repo.


# Tweets Dataset

Tweets are short messages or posts that users share on social media platforms like Twitter. A tweets JSON file provides structured data that can be easily processed and analyzed for extracting insights, conducting research, or building applications.

## Data Dictionary

| Field                     | Data Type    | Description                                                       |
|---------------------------|--------------|-------------------------------------------------------------------|
| _id                       | Object       | An object representing the unique identifier of the tweet.         |
| text                      | String       | The text content of the tweet.                                    |
| in_reply_to_status_id     | Null         | The ID of the status this tweet is replying to, or null if none.   |
| retweet_count             | Null         | The number of times this tweet has been retweeted, or null if none.|
| contributors              | Null         | Contributors associated with the tweet, or null if none.           |
| created_at                | String       | The date and time when the tweet was created.                      |
| geo                       | Null         | Geographic information associated with the tweet, or null if none. |
| source                    | String       | The source or platform from which the tweet was posted.            |
| coordinates               | Null         | The coordinates associated with the tweet, or null if none.        |
| in_reply_to_screen_name   | Null         | The screen name of the user this tweet is replying to, or null if none. |
| truncated                 | Boolean      | Indicates whether the tweet is truncated or not.                   |
| entities                  | Object       | An object containing mentions, URLs, and hashtags in the tweet.    |
| retweeted                 | Boolean      | Indicates whether the tweet has been retweeted or not.             |
| place                     | Null         | Place information associated with the tweet, or null if none.      |
| user                      | Object       | An object representing the user who posted the tweet.              |
| favorited                 | Boolean      | Indicates whether the tweet has been favorited or not.             |
| in_reply_to_user_id       | Null         | The ID of the user this tweet is replying to, or null if none.     |
| id                        | Object       | An object representing the unique identifier of the tweet.         |

## Sample Document

```json
{
  "_id": {
    "$oid": "5c8eccb0caa187d17ca623f5"
  },
  "text": "eu preciso de terminar de fazer a minha tabela, está muito foda **",
  "in_reply_to_status_id": null,
  "retweet_count": null,
  "contributors": null,
  "created_at": "Thu Sep 02 18:11:23 +0000 2010",
  "geo": null,
  "source": "web",
  "coordinates": null,
  "in_reply_to_screen_name": null,
  "truncated": false,
  "entities": {
    "user_mentions": [],
    "urls": [],
    "hashtags": []
  },
  "retweeted": false,
  "place": null,
  "user": {
    "friends_count": {
      "$numberInt": "73"
    },
    "profile_sidebar_fill_color": "768575",
    "location": "",
    "verified": false,
    "follow_request_sent": null,
    "favourites_count": {
      "$numberInt": "1"
    },
    "profile_sidebar_border_color": "1c9dbd",
    "profile_image_url": "http://a2.twimg.com/profile_images/1036412454/OgAAADXK9q6kaxrvfwQTINH66RVLAH9YHb-veRTA4FaWb9KtbGGV_yKTGzmvzTfJidqAb5gK_mpspIE-MIvAASGH2CwAm1T1UIPQk0-HS8x_TV5kdnW30nch7ODk-1_normal.jpg",
    "geo_enabled": false,
    "created_at": "Fri Jul 03 21:44:05 +0000 2009",
    "description": "só os loucos sabem (:",
    "time_zone": "Brasilia",
    "url": "http://http://www.orkut.com.br/Main#Profile?uid=1433295880233078770",
    "screen_name": "Bia_cunha1",
    "notifications": null,
    "profile_background_color": "081114",
    "listed_count": {
      "$numberInt": "0"
    },
    "lang": "en",
    "profile_background_image_url": "http://a1.twimg.com/profile_background_images/133178546/biatwitter.jpg",
    "statuses_count": {
      "$numberInt": "3504"
    },
    "following": null,
    "profile_text_color": "25b8c2",
    "protected": false,
    "show_all_inline_media": false,
    "profile_background_tile": true,
    "name": "Beatriz Helena Cunha",
    "contributors_enabled": false,
    "profile_link_color": "eb55b6",
    "followers_count": {
      "$numberInt": "102"
    },
    "id": {
      "$numberInt": "53507833"
    },
    "profile_use_background_image": true,
    "utc_offset": {
      "$numberInt": "-10800"
    }
  },
  "favorited": false,
  "in_reply_to_user_id": null,
  "id": {
    "$numberLong": "22819396900"
  }
}
```

| Download <img alt="activity status" height="24" src="../../images/download.png" />|
|:---:|
| <a href="tweets.json" ><img src="../../images/dataset.png" ></a>|


## Contribution 🛠️
Please create an [Issue](https://github.com/drshahizan/Python_EDA/issues) for any improvements, suggestions or errors in the content.

You can also contact me using [Linkedin](https://www.linkedin.com/in/drshahizan/) for any other queries or feedback.

[![Visitors](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Fgithub.com%2Fdrshahizan&labelColor=%23697689&countColor=%23555555&style=plastic)](https://visitorbadge.io/status?path=https%3A%2F%2Fgithub.com%2Fdrshahizan)
![](https://hit.yhype.me/github/profile?user_id=81284918)


