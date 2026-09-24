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
    "calculatedPosition": {
      "show": true,
      "size": 100,
      "colorFill": "#C1F5C1/#FA8072"
    },
    "lifePosition": {
      "show": true,
      "size": 31,
      "cost": 89993,
      "currentPrice": 2903,
      "dailyPnl": 434,
      "colorFill": "#C1F5C1/#FA8072"
    },
    "syncSizeButton": {
      "show": true,
      "title": "Увеличить/Уменьшить/Закрыть",
      "colorFill": "#C1F5C1/#FA8072",
      "task": "SyncTickerSize"
    },  
    "calculatedStop": {
      "show": true,
      "size": 31,      
      "stopPrice": 2903,
      "colorFill": "#FAFFB8"      
    },
    "lifeStop": {
      "show": true,
      "size": 31,      
      "stopPrice": 2903,       
      "colorFill": "#FAFFB8" 
    },      
    "syncStopButton": {
      "show": true,
      "title": "Установить/Снять/Синхронизовать",
      "colorFill": "#FAFFB8",
      "task": "SyncTickerStop"
    },
    "syncTickerSizeTask": {
      "show": true,
      "colorFill": "#C1F5C1"
    },      
    "syncTickerStopTask": {
      "show": true,
      "colorFill": "#C1F5C1"
    },           
  ]
}
```

Ответ:
```
{}
```