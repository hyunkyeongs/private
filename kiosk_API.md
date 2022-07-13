# 키오스크 API

* Base URL
```
http://blackhogwarts.com/api/
```


* Method

##### 스토어 목록 (stores)
-> 현재는 베스킨라빈스만 내려옴 (지금은 베라 고정이기때문에 안써도 무관)

```
[
  {
    "id":1,
    "name":"베스킨라빈스",
    "resourceName":"baskin_robbins"
  }
]
```

##### 메뉴 목록 (stores/{id}/menus)

```
[
  {
    "id":1,
    "name":"아이스크림",
    "resourceName":"icon_br_menu_icecream"
  },
  {
    "id":2,
    "name":"아이스크림 케이크",
    "resourceName":"icon_br_menu_icecream_cake"
  },
  {
    "id":3,
    "name":"디저트",
    "resourceName":"icon_br_menu_dessert"
  },
  {
    "id":4,
    "name":"커피",
    "resourceName":"icon_br_menu_coffee"
  },
  {
    "id":5,
    "name":"음료",
    "resourceName":"icon_br_menu_beverage"
  }
]
```


##### 특정 메뉴 내 아이템 목록 (stores/{id}/{menuId}/items)

```
[
  {
    "id":3,
    "menuId":1,
    "name":"싱글레귤러 (콘/컵)",
    "price":3500,
    "resourceName":"icon_br_item_single_regular",
    "maxSelectCount":1,
    "description":"한가지 맛을 센스있게 즐길수 있는 사이즈 (용기무게 제외중량 115g)"
  },
  {
    "id":4,
    "menuId":1,
    "name":"싱글킹 (콘/컵)",
    "price":4300,
    "resourceName":"icon_br_item_single_king",
    "maxSelectCount":1,
    "description":"좋아하는 맛 한가지만 듬뿍 맛볼 수 있는 사이즈 (중량 145g)"
  },
  {
    "id":5,
    "menuId":1,
    "name":"더블주니어 (콘/컵)",
    "price":4700,
    "resourceName":"icon_br_item_double_junior",
    "maxSelectCount":2,
    "description":"두가지 맛을 조금씩 한번에 즐기는 사이즈 (중량 150g)"
  },
  ...
]
```

##### 맛 목록 (stores/{id}/tastes)
-> 스토어에 한정적인 항목이기에 stores 하위로 path 를 설정

```
[
  {
    "id":1,
    "name":"31요거트",
    "resourceName":"icon_br_taste_31_yogurt",
    "ranking":0
  },
  {
    "id":2,
    "name":"아몬드 봉봉",
    "resourceName":"icon_br_taste_almond",
    "ranking":2
  },
  {
    "id":3,
    "name":"애플민트",
    "resourceName":"icon_br_taste_apple_mint",
    "ranking":0
  },
  {
    "id":4,
    "name":"블랙 소르베",
    "resourceName":"icon_br_taste_black_sherbet",
    "ranking":0
  },
  {
    "id":5,
    "name":"체리 쥬빌레",
    "resourceName":"icon_br_taste_cherry",
    "ranking":0
  },
  {
    "id":6,
    "name":"치코치코 치코리타",
    "resourceName":"icon_br_taste_chico",
    "ranking":0
  },
...
]
```

