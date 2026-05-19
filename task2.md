Задание 2: Проектирование API





REST API запрос



```http

GET /api/v1/partner-stores?latitude=55.7558\&longitude=37.6173\&limit=20 HTTP/1.1

Host: api.petruka-zelenaya.ru

Authorization: Bearer <access\_token>

Accept: application/json

Accept-Language: ru

X-App-Version: 2.4.1



_______________________________________________________


Ответ


{
  "status": "200",
  "data": [
    {
      "id": "store_metro_01",
      "name": "METRO",
      "delivery_window": "Сегодня 21:00–23:00",
      "delivery_type": "scheduled",
      "logo_url": "https://........../metro.webp",
      "external_link": "https://partner.metro.ru/store/01"
    },
    {
      "id": "store_auchan_04",
      "name": "Ашан",
      "delivery_window": "Сегодня 18:00–20:00",
      "delivery_type": "scheduled",
      "logo_url": "https://........../auchan.webp",
      "external_link": "https://partner.auchan.ru/store/04"
    },
    {
      "id": "store_vkusvill_09",
      "name": "ВкусВилл",
      "delivery_window": "От 20 до 60 минут",
      "delivery_type": "express",
      "logo_url": "https://........../vkusvill.webp",
      "external_link": "https://partner.vkusvill.ru/store/09"
    }
    {
      "id": "store_viktoria_11",
      "name": "ВИКТОРИЯ",
      "delivery_window": "Сегодня 17:00–19:00",
      "delivery_type": "scheduled",
      "logo_url": "https://........../viktoria.webp",
      "external_link": "https://partner.viktoria.ru/store/11"
    }
  ],
  "meta": {
    "total": 42,
    "limit": 20,
    "offset": 0,
    "sorted_by": "distance_asc"
  }
}





