### Terminal

Метод получения терминала управления портфелем

*api/trader-finam/task/cancel*

Запрос:
```
{
  "totalSum": 909536.54,
  "money": 156.05,
  "totalDailyPnl": 9095.04,  
  "terminalRows": [
    "ticker": "HEAD",
    "targetPosition": {
      "show": true,
      "size": 100,
      "colorFill": ""
    },
    "lifePosition": {
      "show": true,
      "size": 31,
      "colorFill": "",
      "cost": 89993,
      "currentPrice": 2903,
      "dailyPnl": 434
    },
    "syncSizeButton": {
      "show": true,
      "title": "Увеличить/Уменьшить/Закрыть",
      "colorFill": "",
      "task": "SyncTickerSize"
    },  
    "targetStop": {
      "show": true,
      "size": 31,      
      "stopPrice": 2903,
      "colorFill": ""      
    },
    "lifeStop": {
      "show": true,
      "size": 31,      
      "stopPrice": 2903,       
      "colorFill": "" 
    },      
    "syncStopButton": {
      "show": true,
      "title": "Установить/Снять/Изменить",
      "colorFill": "",
      "task": "SyncTickerStop"
    },
    "syncTickerSizeTask": {
      "show": true,
      "state": "New",
      "colorFill": "",
      "task": "SyncTickerSize"
    },      
    "syncTickerStopTask": {
      "show": true,
      "state": "New",
      "colorFill": "",
      "task": "SyncTickerStop"
    },           
  ]
}
```

Ответ:
```
{}
```