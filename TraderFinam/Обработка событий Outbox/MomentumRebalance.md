## MomentumRebalance
Ребалансировка портфеля Моментум

#### Пример
```
{
  "id": "80a82306-e32a-40ae-aecc-7645d0cd0e01",
  "source": "Momentum",
  "type": "MomentumRebalance",
  "ticker": "SBER;LKOH;NVTK;FMMM",
  "share": "0.1;0.1;0.1;0.7",
  "state": "New",
  "createAt": "2026.09.20 00:00:00",
  "updatedAt": "2026.09.20 00:00:00",
  "completedAt": "2026.09.20 00:00:00"
}
```

#### Обработка
1. Перевести текущее событие **MomentumRebalance** в статус *InProgress*
2. Перевести событие **ControlLiquidityPosition** в статус *Completed* (убираем контроль за FMMM)
3. Добавить событие **MomentumSyncLiquidityPosition** с полями:
   - *State = New*
4. Для каждого тикера добавить событие **MomentumSyncTickerPosition** с полями:
   - *State = New*
5. Добавить событие **ControlLiquidityPosition** с полями:
   - *State = New*
6. Перевести текущее событие **MomentumRebalance** в статус *Completed*
