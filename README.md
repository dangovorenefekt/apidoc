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

#### GE Pods DB and Episodes DB Calls - No Authenticatiin Required

<details> <summary><code>GET</code> <code><b>/v1/episodes/last-ten</b></code> <code>(gets last ten episodes added to Episodes DB)</code></summary>

##### Parameters

> None

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           | application/json                  | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/last-ten   
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
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/random-pod
> ```

##### Rate limit

> 10 r/m

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/episodes/[int:geid]</b></code> <code>(gets podcast episode by gied from Episodes DB)</code></summary>

##### Parameters

> None

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/8700
> ```

##### Rate limit

> 10 r/m

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/podcasts</b></code> <code>(gets podcast data about Podcast DB)</code></summary>

##### Parameters

> none    

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/podcasts
> ```

##### Rate limit

> 10 r/m

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
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/podcasts/426
> ```

##### Rate limit

> 10 r/m

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/podcasts/[int:podcast-id]/episodes</b></code> <code>(gets all episodes from Episode DB for requested podcast-id)</code></summary>

##### Parameters

> none    

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           |  application/json                 | JSON                                                                |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/podcasts/426/episodes
> ```

##### Rate limit

> 10 r/m

</details>

------------------------------------------------------------------------------------------
