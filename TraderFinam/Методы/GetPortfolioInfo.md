### GetPortfolioInfo

Метод получения текущего состояния портфеля

*api/trader-finam/portfolio-info*

Запрос:
```
{}
```

Ответ:
```
{
  "totalSum": 909536.54,
  "money": 156.05,
  "totalDailyPnl": 9095.04,
  "positions": [
    {
      "ticker": "HEAD",
      "size": 31,
      "cost": 89993,
      "currentPrice": 2903,
      "dailyPnl": 434
    },
    {
      "ticker": "FMMM",
      "size": 26554,
      "cost": 368702.29,
      "currentPrice": 13.885,
      "dailyPnl": 132.77
    }
  ]
}
```