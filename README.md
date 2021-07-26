## Govoren Efekt API

#### Available DB Columns

<details><summary>Pods DB:</summary>

> | filed       | type    | desciption                            | API Exposed |
> |-------------|---------|---------------------------------------|-------------|
> | podcast_id  | INTEGER | PRIMARY KEY, Podcast ID in GE Pods DB | No          |
> | title       | TEXT    | Podcast Name                          | No          |
> | description | TEXT    | Podcast Description                   | No          |
> | website     | TEXT    | Podcast Website Link                  | No          |
> | rssfeed     | TEXT    | Podcast RSS Feed Link                 | No          |
> | etag        | TEXT    | RSS Feed Latest etag                  | No          |
> | modified    | TEXT    | Last-Modified from RSS Feed           | No          |

</details>

------------------------------------------------------------------------------------------

#### GE Episodes Database Calls - No Authenticatiin Required

<details> <summary><code>GET</code> <code><b>/v1/episodes/last-ten</b></code> <code>(gets last ten episodes added to Episodes DB)</code></summary>

##### Parameters

> None

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | 200           | application/json                  | JSON string                                                         |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/last-ten' 
> ```

</details>

<details>
 <summary><code>GET</code> <code><b>/v1/episodes/random-pod</b></code> <code>(gets random podcast episode from Episodes DB)</code></summary>

##### Parameters

> None

##### Responses

> | http code     | content-type                      | response                                                            |
> |---------------|-----------------------------------|---------------------------------------------------------------------|
> | `200`         | `application/json`                | JSON string                                                         |

##### Example cURL

> ```javascript
>  curl --location --request GET 'https://api.govorenefekt.bg/v1/episodes/random-pod'
> ```

</details>

------------------------------------------------------------------------------------------
