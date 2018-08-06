# Data Of Watchout

## Release Notes

### 2018/08/06

- 發佈資料格式版本 v1.0.0
- 新增「各城市下各候選人相關之最熱門提問」資料集

## Datasets

### ask/2018-mayor/candidate-popular-questions

[給問擂台] 各城市下各參選人相關之最熱門提問

### 資料位置

- [台北市](https://data.watchout.tw/ask/2018-mayor/2018-taipei-candidate-popular-questions.json)
- [新北市](https://data.watchout.tw/ask/2018-mayor/2018-new-taipei-candidate-popular-questions.json)
- [桃園市](https://data.watchout.tw/ask/2018-mayor/2018-taoyuan-candidate-popular-questions.json)
- [台中市](https://data.watchout.tw/ask/2018-mayor/2018-taichung-candidate-popular-questions.json)
- [台南市](https://data.watchout.tw/ask/2018-mayor/2018-tainan-candidate-popular-questions.json)
- [高雄市](https://data.watchout.tw/ask/2018-mayor/2018-kaohsiung-candidate-popular-questions.json)

### 資料格式說明

#### 範例

``` json
}
  "formatVersion": "資料格式版本號碼", //資料格式版本號碼
  "lastBuildDate": 1533522837782, //資料最後更新時間
  "uuid": "ask-2018-mayor-candidatePopularQuestions-2018-taichung-1533522837782", //資料uuid
  "data": [
    {
      "candidate": { //參選人資料
        "url": "https://park.watchout.tw/personas/218", //參選人個人頁面
        "name": "林佳龍", //參選人姓名
        "party": { //參選人所屬政黨資訊
          "name": "民主進步黨", //所屬政黨名稱
          "abbreviation": "民進黨", //所屬政黨縮寫
          "color": "#009A00" //所屬政黨代表色
        },
        "questions": [ //參選人相關提問
          {
            "url": "https://ask.watchout.tw/games/2018-taichung/questions/648", //提問網址
            "topic": "性別", //提問議題類別 [註1]
            "title": "兩位對於台中市性別與同志平權議題的想法？會有什麼支持政策？", //提問標題
            "content": "今年年底的公投有婚姻平權公投，也表示同志議題與相 ...\n", //提問內容
            "push": 128, //目前連署數
            "threshold": 100 //連署門檻
          },
  ]
}
```

註1: [議題類別清單API](https://core.watchout.tw/park/topics?type=watchout)