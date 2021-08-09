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

#### GE Episodes Database Calls - No Authenticatiin Required

<details> <summary><code>GET</code> <code><b>/v1/episodes/last-ten</b></code> <code>(gets last ten episodes added to Episodes DB)</code></summary>

##### Parameters

> None

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           | application/json                  | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/last-ten' 
> ```

##### Rate Limit

> None

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/episodes/random-pod</b></code> <code>(gets random podcast episode from Episodes DB)</code></summary>

##### Parameters

> None

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/random-pod'
> ```

##### Rate limit

> 10 r/m

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/podcasts</b></code> <code>(gets podcast data from Podcast DB)</code></summary>

##### Parameters

> none    
> podcast_id - integer, if send will return podcast data from Podcast DB

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/podcasts?podcast_id=462'
> ```

##### Rate limit

> 10 r/m

</details>

------------------------------------------------------------------------------------------
