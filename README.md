## Govoren Efekt API

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/U7U51VFGK)

#### Available DB 

<details><summary><code>Pods DB</code></summary>   


> | column      | type    | desciption                               | API Exposed |
> |-------------|---------|------------------------------------------|-------------|
> | podcast_id  | INTEGER | Podcast ID in GE Pods DB                 | Yes         |
> | title       | TEXT    | Podcast Name                             | Yes         |
> | description | TEXT    | Podcast Description                      | Yes         |
> | website     | TEXT    | Podcast Website Link                     | Yes         |
> | rssfeed     | TEXT    | Podcast RSS Feed Link                    | Yes         |
> | etag        | TEXT    | RSS Feed Latest etag                     | No          |
> | modified    | TEXT    | Last-Modified from RSS Feed              | No          |
> | category    | TEXT    | Podcast Category                         | Yes         |
> | lastep      | TEXT    | Lastest episode                          | No          |
</details>

<details><summary><code>Episodes DB</code></summary>   
 

> | column      | type    | desciption                                | API Exposed |
> |-------------|---------|-------------------------------------------|-------------|
> | geid        | INTEGER | Episode ID in GE Episode DB               | Yes         |
> | guid        | TEXT    | Episode GUID                              | Yes         |
> | podcast_id  | INTEGER | Podcast ID in GE Pods DB                  | Yes         |
> | link        | TEXT    | Episode Link                              | Yes         |
> | audio       | TEXT    | Link to Episode Audio                     | Yes         |
> | image       | TEXT    | Link to Episode Image                     | Yes         |
> | title       | TEXT    | Episode Title                             | Yes         |
> | description | TEXT    | Epispde Description                       | Yes         |
> | pubdate     | TEXT    | Episode Publication Date                  | Yes         |
> | isodate     | TEXT    | Episode Publication Date converted to ISO | No          |
> | duration    | TEXT    | Episode Duration                          | Yes         |
> | explicit    | TEXT    | Aadult Language or Sexual Content         | Yes         |
> | lenght      | TEXT    | Episode Lenght in bytes                   | Yes         |
> | author      | TEXT    | Episode Author                            | Yes         |
> | episodeno   | TEXT    | Episode number (Podcast Internal)         | Yes         |
> | seasonno    | TEXT    | Episode Season Number (Podcast Internal)  | Yes         |

</details>

------------------------------------------------------------------------------------------

#### GE Pods DB and Episodes DB Calls

<details> <summary><code>GET</code> <code><b>/v1/stats</b></code> <code>(This call returns some statistics about Pods and Episodes DB)</code></summary>

##### Parameters

> none

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           | application/json                  | JSON                                                                |
> | 429           | application/json                  | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/stats'   
> ```

##### Rate Limit

> None

##### Example reply

> ```javascript
>  {   
>    "stats": {   
>        "feedCountTotal": 439,   
>        "episodeCountTotal": 16800,   
>        "NewEpisodes3days": 47,   
>        "NewEpisodes10days": 144,   
>        "NewEpisodes30days": 475,   
>        "NewEpisodes90days": 1371   
>    },   
>    "as-of": "2022-03-26 19:52:03.598625"   
> } 
> ```

</details>

<details> <summary><code>GET</code> <code><b>/v1/episodes</b></code> <code>(This call returns some statistics about Episodes DB)</code></summary>

##### Parameters

> none

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           | application/json                  | JSON                                                                |
> | 429           | application/json                  | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes'   
> ```

##### Rate Limit

> None

##### Example reply

> ```javascript
>{
>    "stats": {
>        "episodesCountTotal": 16801,
>        "as-of": "2022-03-26 22:07:36.801073"
>    }
>}
> ```
</details>

<details> <summary><code>GET</code> <code><b>/v1/episodes/recent</b></code> <code>(This call returns the most recent _max_ number of episodes from Episodes DB)</code></summary>

##### Parameters

> max - Maximum number of results to return. (optional | default: 10 | min: 1 | max: 10)

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           | application/json                  | JSON                                                                |
> | 429           | application/json                  | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/recent?max=1'   
> ```

##### Rate Limit

> None

##### Example reply

> ```javascript
>{
>    "items": [
>        {
>            "podcast_name": "Dir Podcast",
>            "category": "News",
>            "geid": 20289,
>            "guid": "c0bea2da-32c1-4135-a667-4cf3fd2048dc",
>            "podcast_id": 476,
>            "link": "https://anchor.fm/dirbg/episodes/Podcast-e1iodhj",
>            "audio": "https://anchor.fm/s/4515cc74/podcast/play/52229107/https%3A%2F%2Fd3ctxlq1ktw2nl.cloudfront.net%2Fstaging%2F2022-4-19%2F266520291-44100-2-0ff2defd56ff8.m4a",
>            "image": "https://d3t3ozftmdmh3i.cloudfront.net/production/podcast_uploaded_episode/11490565/11490565-1652951137867-235309615d455.jpg",
>            "title": "\"Не\" на металните решетки на входа на Народното събрание, казват Podcast слушателите",
>            "description": "<p>Коментирайте на PodcastNews@dir.bg</p>\n<p>Това са обедните Podcast новини на 19.05.2022 г.</p>",
>            "pubdate": "Thu, 19 May 2022 09:05:43 GMT",
>            "duration": "13:26",
>            "explicit": null,
>            "length": "13040102",
>            "author": "Dir.bg",
>            "episodeno": "",
>            "seasonno": "",
>            "player": "https://podcastalot.com/playb/20289",
>            "uri": "https://api.govorenefekt.bg/v1/episodes/by-geid/20289"
>        }
>    ],
>    "count": 1
>}
> ```
</details>

<details>
 <summary><code>GET</code> <code><b>/v1/episodes/random</b></code> <code>(gets random podcast episode from Episodes DB)</code></summary>

##### Parameters

> max - Maximum number of results to return. (optional | default: 1 | min: 1 | max: 10)

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/random?max=3'
> ```

##### Rate limit

> 10 r/m

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/episodes/by-geid/[int:geid]</b></code> <code>(gets podcast episode by gied from Episodes DB)</code></summary>

##### Parameters

> geid - integer, episode GEID in Episodes DB

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/by-geid/8700'
> ```

##### Rate limit

> 10 r/m

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/episodes/by-date/[string:pubdate]</b></code> <code>(gets podcast episodes published on the date)</code></summary>

##### Parameters

> geid - string, date in format YYYYMMDD

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/by-date/20201222'
> ```

##### Rate limit

> 10 r/m

</details>

<details> <summary><code>GET</code> <code><b>/v1/podcasts</b></code> <code>(This call returns some statistics about Pods DB)</code></summary>

##### Parameters

> none

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           | application/json                  | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/podcasts'   
> ```

##### Rate Limit

> None

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/podcasts/[int:podcast-id]</b></code> <code>(gets data about requested podcast-id from Podcast DB)</code></summary>

##### Parameters

> none    

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/podcasts/426'
> ```

##### Rate limit

> 10 r/m

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/podcasts/[int:podcast-id]/episodes</b></code> <code>(gets all episodes from Episode DB by podcast-id)</code></summary>

##### Parameters

> none    

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/podcasts/426/episodes'
> ```

##### Rate limit

> 10 r/m

</details>

------------------------------------------------------------------------------------------
