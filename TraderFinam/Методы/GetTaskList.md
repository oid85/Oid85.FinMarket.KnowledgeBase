### GetTaskList

Метод получения текущих заданий outbox

*api/trader-finam/task/list*

Запрос:
```
{}
```

Ответ:
```
{
  "tasks": [
    {
      "id": "80a82306-e32a-40ae-aecc-7645d0cd0e01",
      "source": "Momentum",
      "type": "SyncTicker",
      "ticker": "SBER",      
      "targetSize": "100",
      "state": "New",
      "createAt": "2026.09.20 00:00:00",
      "updatedAt": "2026.09.20 00:00:00",
      "completedAt": "2026.09.20 00:00:00"
    }
  ]
}
```