<details><summary>Episodes endpoints</summary>

<details><summary>Episodes by date</summary>

##### Request
> ```javascript
> https --follow --timeout 3600 GET 'api.govorenefekt.bg/v1/episodes/by-date/20220101' x-api-key:'dc4f3ce4-f0fa-45f7-bc83-bc16477bc6e6'
> ```

##### Response
> ``` javascript
>  {
>      "count": 4,
>      "items": [
>	  {
>	      "geid": 13804,
>	      "guid": "3e9624de-71c6-4b26-9508-eb7e39b17fd5",
>	      "podcast_id": 242,
>	      "podcast_name": "Изпразнен Град",
>	      "link": "https://anchor.fm/izpraznen-grad/episodes/51---e1ccoes",
>	      "audio": "https://anchor.fm/s/481e0940/podcast/play/45555612/https%3A%2F%2Fd3ctxlq1ktw2nl.cloudfront.net%2Fstaging%2F2022-0-1%2F3729b95a-37e0-765b-fe7b-14fb49a2c7b0.mp3",
>	      "image": "https://d3t3ozftmdmh3i.cloudfront.net/production/podcast_uploaded_nologo400/11999280/11999280-1610796346362-701de25c5ee78.jpg",
>	      "title": "Еп 51 - Дебел г*з",
>	      "description": "<p>&nbsp;</p>",
>	      "pubdate": "Sat, 01 Jan 2022 10:00:48 GMT",
>	      "duration": "1:00:18",
>	      "explicit": null,
>	      "length": "115801364",
>	      "author": "Izpraznen Grad",
>	      "episodeno": "51",
>	      "seasonno": "1",
>	      "uri": "https://api.govorenefekt.bg/v1/episodes/by-geid/13804",
>	      "player": "https://podcastalot.com/playb/13804"
>	  },
>	  {
>	      "geid": 13805,
>	      "guid": "e82077f5-811b-4ddf-b026-369ba9c64e05",
>	      "podcast_id": 44,
>	      "podcast_name": "Животът е Прекрасен с Милена Голева",
>	      "link": "https://anchor.fm/milenagoleva/episodes/ep-e1ccsmg",
>	      "audio": "https://anchor.fm/s/435825bc/podcast/play/45559952/https%3A%2F%2Fd3ctxlq1ktw2nl.cloudfront.net%2Fstaging%2F2022-0-1%2F240263630-44100-2-199644357c73c.m4a",
>	      "image": "https://d3t3ozftmdmh3i.cloudfront.net/production/podcast_uploaded_nologo400/11198503/11198503-1634300755727-9f452d4973205.jpg",
>	      "title": "❤️ Продуктивно ново начало! Нова Луна в Козирог!",
>	      "description": "<p>🙏 БлагоДаря за подкрепата, положителното отношение и заедността! ❤️ Медитация по Новолуние: https://milenagoleva.com/izlekuvay-svoya-zhivot-tehnika-za-privlichane-na-izobilie/💎 Колекция авторски водени медитации от Милена Голева: https://milenagoleva.com/product-category/vodenimeditacii/vodeni-meditacii-digitalni/❤️ Онлайн семинари с Милена Голева: https://milenagoleva.com/onlayn-seminar/❤️ Авторска програма Парите и науката за Вибрациите: https://milenagoleva.com/parite-i-naukata-za-vibratsiite/❤️ Онлайн йога студио с Милена Голева: https://milenagoleva.com/online-yoga-s-milena-goleva/❤️ Групата ни в Instagram: https://www.instagram.com/milenagoleva_official/❤️ Групата ни в You Tube: https://www.youtube.com/c/МиленаГолева❤️ Групата ни във Facebook: https://www.facebook.com/milenagolevaofficial❤️ Spotify: https://open.spotify.com/show/5s6NQbTpqesmw4op28Jl0d?si=wyTuwInYToCENNSY_0OCYA❤️ Apple Podcast: https://podcasts.apple.com/bg/podcast/%D0%B6%D0%B8%D0%B2%D0%BE%D1%82%D1%8A%D1%82-%D0%B5-%D0%BF%D1%80%D0%B5%D0%BA%D1%80%D0%B0%D1%81%D0%B5%D0%BD-%D1%81-%D0%BC%D0%B8%D0%BB%D0%B5%D0%BD%D0%B0-%D0%B3%D0%BE%D0%BB%D0%B5%D0%B2%D0%B0/id1543778811❤️ Google Podcast: https://podcasts.google.com/feed/aHR0cHM6Ly9hbmNob3IuZm0vcy80MzU4MjViYy9wb2RjYXN0L3Jzcw?sa=X&amp;ved=2ahUKEwjuy5vqnczzAhVkVeUKHdL6B14Q9sEGegQIARAC</p>",
>	      "pubdate": "Sat, 01 Jan 2022 14:24:46 GMT",
>	      "duration": "48:54",
>	      "explicit": null,
>	      "length": "47458541",
>	      "author": "Milena Goleva",
>	      "episodeno": "",
>	      "seasonno": "",
>	      "uri": "https://api.govorenefekt.bg/v1/episodes/by-geid/13805",
>	      "player": "https://podcastalot.com/playb/13805"
>	  },
>	  {
>	      "geid": 13807,
>	      "guid": "bb62c114-5cfd-448d-b0ba-b295dc8b858c",
>	      "podcast_id": 259,
>	      "podcast_name": "Три Мазета",
>	      "link": "https://anchor.fm/tri-mazeta/episodes/94-----award-show-2021-e1cae8k",
>	      "audio": "https://anchor.fm/s/17251c20/podcast/play/45479636/https%3A%2F%2Fd3ctxlq1ktw2nl.cloudfront.net%2Fstaging%2F2021-11-30%2F16b45038-b491-a584-4ea9-00e16eee4dff.mp3",
>	      "image": "https://d3t3ozftmdmh3i.cloudfront.net/production/podcast_uploaded_nologo400/3783080/3783080-1584914004462-f9d28fe188234.jpg",
>	      "title": "Епизод #94 - Три Мазета award show 2021",
>	      "description": "<p>Честита Нова Година на всички! И за да затоврим 2021 година си спретнахме леко импровизирани награди за най-лоши, най-добри и най-криндж филми, игри, сериали и прочие.</p>\n<p>Пишете ни на trimazeta@gmail.com и ни последвайте тук:</p>\n<p><a href=\"https://www.facebook.com/trimazeta\">facebook </a>- https://www.facebook.com/trimazeta</p>\n<p><a href=\"https://www.youtube.com/channel/UCXxbKGELoSYiCy_Q7ExDgXQ\">youtube</a> - https://www.youtube.com/channel/UCXxbKGELoSYiCy_Q7ExDgXQ</p>\n<p>Timestamps:</p>\n<p>00:00 Начало</p>\n<p>01:15 Писмо за тирове</p>\n<p>04:45 Писмо за spotify wrapped</p>\n<p>09:30 Писмо кореспонденция за NFT</p>\n<p>25:50 Започва класацията: Worst video game remaster</p>\n<p>30:20 Best &amp; Worst movie</p>\n<p>45:00 Best &amp; Worst TV show</p>\n<p>54:35 Worst comic book movie or TV show</p>\n<p>1:00:05 Най-лош акцент</p>\n<p>1:03:08 Най-голям криндж</p>\n<p>1:08:25 Най-лоша перука, коса или грим</p>\n<p>1:13:00 Worst sequel or franchise</p>\n<p>1:17:13 Most generic movie</p>\n<p>1:18:55 Best Fast &amp; Furious character</p>\n<p>1:19:50 Best anime</p>\n<p>1:23:15 Most &amp; Least anticipated movie or TV show</p>\n<p>1:27:50 Most anticipated game</p>\n<p>1:30:32 Най-атрактивни дестинация за 2021 година</p>\n<p>1:33:45 Спортно събитие на 2021</p>\n<p>1:37:50 Най-глупаво звучащо ИМЕ на Isekai Anime</p>\n<p>1:43:50 Best NFT</p>\n<p>1:46:23 Best Три Мазета episode</p>",
>	      "pubdate": "Sat, 01 Jan 2022 23:00:00 GMT",
>	      "duration": "1:51:26",
>	      "explicit": null,
>	      "length": "105538123",
>	      "author": "Три Мазета",
>	      "episodeno": "1",
>	      "seasonno": "4",
>	      "uri": "https://api.govorenefekt.bg/v1/episodes/by-geid/13807",
>	      "player": "https://podcastalot.com/playb/13807"
>	  },
>	  {
>	      "geid": 18618,
>	      "guid": "b32a123d-5bd4-49e0-8fcc-92e057ab06eb",
>	      "podcast_id": 527,
>	      "podcast_name": "Пътят на родителя",
>	      "link": "https://anchor.fm/maria-petrova7/episodes/ep-e1cakum",
>	      "audio": "https://anchor.fm/s/78ee69e8/podcast/play/45486486/https%3A%2F%2Fd3ctxlq1ktw2nl.cloudfront.net%2Fstaging%2F2021-11-30%2F8ece85a4-bd56-9e4d-e2f8-891582eb6d20.mp3",
>	      "image": "https://d3t3ozftmdmh3i.cloudfront.net/production/podcast_uploaded_episode/20188906/20188906-1641288230481-2aa452a0e9bf.jpg",
>	      "title": "Какво ни дава изграждането на рутина?",
>	      "description": "Аз съм израстнала със съставяне на график и следването му. И дори и сега обичам да планирам и да имам предсказуемост. Но не всички родители обичат повторението и понякога е трудно да създадат постоянен ритъм. В този епизод, отговарям на два въпроса: \"Какво ни дава рутината?\" и \"Защо е важна за децата?\" и се надявам, че това може да помогне да погледнете на рутината с други очи.\nМоже да споделяте вашите истории, предложения и обратна връзка в страницата в Instagram (parentpath) и Facebook (Пътят на родителя) или на имейл: kirchevamariya@gmail.com.",
>	      "pubdate": "Sat, 01 Jan 2022 19:37:41 GMT",
>	      "duration": "14:49",
>	      "explicit": null,
>	      "length": "12487740",
>	      "author": "Мария Петрова",
>	      "episodeno": "5",
>	      "seasonno": "1",
>	      "uri": "https://api.govorenefekt.bg/v1/episodes/by-geid/18618",
>	      "player": "https://podcastalot.com/playb/18618"
>	  }
>      ]
>  }
> ```
</details>

<details><summary>Episodes by geid</summary>

##### Request
> ```javascript
> https --follow --timeout 3600 GET 'api.govorenefekt.bg/v1/episodes/by-geid/512' x-api-key:'dc4f3ce4-f0fa-45f7-bc83-bc16477bc6e6'
> ```

##### Response
> ``` javascript
> {
>    "items": [
>        {
>            "podcast_name": "Сутрешно предаване за мениджъри с Пламен Петров",
>            "category": "Education,Business,Management,Business",
>            "geid": 512,
>            "guid": "http://rss.castbox.fm/everest/album-687807c0a0424b2a8592389a43bd74b9-cc0ac0d4a68b49bea640070ccb15fe86",
>            "podcast_id": 12,
>            "link": "http://rss.castbox.fm/everest/album-687807c0a0424b2a8592389a43bd74b9-cc0ac0d4a68b49bea640070ccb15fe86",
>            "audio": "https://s3.castbox.fm/c5/4a/73/4d193242539f53eb8c868713c6.mp3",
>            "image": "https://s3.castbox.fm/7f/f5/9c/634d254b0dac4d41712a10ba5d.jpg",
>            "title": "6 от 75 глава на Аудио #книгастудендушзамениджъри",
>            "description": "6 от 75 глава на Аудио #книгастудендушзамениджъри \n\n---\nКнига \"Студен душ за мениджъри\" - http://www.equinox-partners.bg/cold-shower-for-managers-book.html\n\nХаштаг на книгата в LinkedIn и другите социални мрежи: #книгастудендушзамениджъри\n\nЕднодневно обучение за мениджъри \"Мотивация и ефективна комуникация\" - http://www.equinox-partners.bg/effective-communication-and-motivation-for-managers.html\n\n3-месечни лидерски програми (само затворени по поръчка на една компания) - http://www.equinox-partners.bg/management-development-program.html",
>            "pubdate": "Sat, 27 Jul 2019 18:23:03 +0000",
>            "duration": "00:01:44",
>            "explicit": null,
>            "length": "1251056",
>            "author": "",
>            "episodeno": "",
>            "seasonno": "",
>            "player": "https://podcastalot.com/playb/512"
>        }
>    ]
> }
> ```
</details>

<details><summary>Random episode</summary>

##### Request
> ```javascript
> https --follow --timeout 3600 GET 'api.govorenefekt.bg/v1/episodes/random?max=3'
> ```

###### Response
> ``` javascript
> {
>     "count": 3,
>     "items": [
>         {
>             "podcast_name": "Уроци за успех - Капитал подкаст",
>             "category": "News & Politics",
>             "geid": 13004,
>             "guid": "https://www.capital.bg/podcast/uroci_za_uspeh/2021/12/10/4289285_goliamata_promiana_ne_e_edno_subitie/",
>             "podcast_id": 477,
>             "link": "https://www.capital.bg/podcast/uroci_za_uspeh/2021/12/10/4289285_goliamata_promiana_ne_e_edno_subitie/",
>             "audio": "https://feeds.soundcloud.com/stream/1170545785-capital-podcasts-golyamata-promyana-ne-e-edno-sbitie.mp3",
>             "image": "http://www.capital.bg/standalone/podcast/images/uu.jpg",
>             "title": "\"Голямата промяна не е едно събитие\"",
>             "description": "Старши вицепрезидентът в SAP Румяна Тренчева в подкаста &quot;Уроци за успех&quot;",
>             "pubdate": "Fri, 10 Dec 2021 00:00:00 +0200",
>             "duration": "00:25:42",
>             "explicit": "0",
>             "length": "",
>             "author": "338",
>             "episodeno": "",
>             "seasonno": "",
>             "player": "https://podcastalot.com/playb/13004"
>         },
>         {
>             "podcast_name": "Magi San & Dimikask PODCAST",
>             "category": "Comedy",
>             "geid": 1445,
>             "guid": "2f7776c4-9f50-2d1b-149b-9cc3f31531ef",
>             "podcast_id": 69,
>             "link": "https://anchor.fm/magdalena-aleksandrova/episodes/ep-e1do40",
>             "audio": "https://anchor.fm/s/3441b5c/podcast/play/499264/https%3A%2F%2Fd3ctxlq1ktw2nl.cloudfront.net%2Fstaging%2F2020-02-12%2F1b7a611048614d8560fcea0f5e3f96a2.m4a",
>             "image": "https://d3t3ozftmdmh3i.cloudfront.net/production/podcast_auto/447951/447951-1525372215295-26-FFFFFF.jpg",
>             "title": "Започваме ПОДКАСТ!",
>             "description": "Ние сме Маги и Дими - партньори в живота и в този нов подкаст! Може би ни познавате от YouTube и каналите Magi San & Dimikask. Тук обаче видеото ще остане на заден план, защото ще си говорим. За какво ли? Темите ще се въртят главно около взаимоотношенията в една двойка, домашната хармония, компромисите, отглеждането на КОТЕ и планирането на светло бъдеще. Както се казва - stay tuned! Това е само едно простичко 10-минутно хаотично подкастче като за старт. Предстоят доста по-дълги, тематични подкастове :)",
>             "pubdate": "Thu, 03 May 2018 18:29:37 GMT",
>             "duration": "10:52",
>             "explicit": null,
>             "length": "10550581",
>             "author": "Magi San",
>             "episodeno": "",
>             "seasonno": "",
>             "player": "https://podcastalot.com/playb/1445"
>         },
>         {
>             "podcast_name": "Жълто- Освежи Бизнеса Си",
>             "category": "Business,Marketing",
>             "geid": 15759,
>             "guid": "05c4fa5f-f769-4f6a-8bca-3354f36c1d6b",
>             "podcast_id": 324,
>             "link": "https://anchor.fm/zyltomarketing/episodes/ep-egjo0u",
>             "audio": "https://anchor.fm/s/2b563fbc/podcast/play/16424414/https%3A%2F%2Fd3ctxlq1ktw2nl.cloudfront.net%2Fproduction%2F2020-6-11%2F89340009-44100-2-4ecbb4650c6fa.mp3",
>             "image": "https://d3t3ozftmdmh3i.cloudfront.net/production/podcast_uploaded/7170727/7170727-1594482415712-566d474d07062.jpg",
>             "title": "Добре дошли!",
>             "description": "Какво ще намериш тук- накратко разказвам за този канал. Заповядай във Фейсбук Жълто-освежи бизнеса си и в Инстаграм @zyltomarketig",
>             "pubdate": "Sat, 11 Jul 2020 15:40:56 GMT",
>             "duration": "03:30",
>             "explicit": null,
>             "length": "3398230",
>             "author": "Жълто с Леда",
>             "episodeno": "1",
>             "seasonno": "",
>             "player": "https://podcastalot.com/playb/15759"
>         }
>     ]
> }
> ```
</details>


</details>
