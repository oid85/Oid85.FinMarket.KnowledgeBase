### MomentumRebalance
Ребалансировка портфеля Моментум

#### Пример

```
{
  "id": "80a82306-e32a-40ae-aecc-7645d0cd0e01",
  "order": null,
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
2. Перевести событие **ControlLiquidityPosition** в статус *Pause* (убираем контроль за FMMM)
3. Добавить событие **MomentumSyncLiquidityPosition** с полями:
   - *State = New*
   - *Order = 1*
4. Для каждого тикера добавить событие **MomentumSyncTickerPosition** с полями:
   - *State = New*
   - *Order* - следующий в порядке возрастания
5. Добавить событие **MomentumSyncLiquidityPosition** с полями:
   - *State = New*
   - *Order* - следующий в порядке возрастания
6. Перевести текущее событие **MomentumRebalance** в статус *Completed*

### MomentumSyncLiquidityPosition
Синхронизация позиции по денежному рынку (FMMM)
1. Снять все активные заявки по тикеру FMMM
2. Получить полную стоимость портфеля
3. Расчитать целевой размер позиции FMMM
4. Докупить или допродать до целевого размера

#### Пример

#### Обработка

### MomentumSyncTickerPosition
Синхронизация позиции по тикеру

#### Пример

#### Обработка

### ControlLiquidityPosition
Проверка, можно ли докупить FMMM на остаток денежных средств в портфеле

#### Пример

#### Обработка