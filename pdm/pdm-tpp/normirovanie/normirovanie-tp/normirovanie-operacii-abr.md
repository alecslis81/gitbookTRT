---
description: Инструкция по нормированию операций сборки на РЦ LEAS
---

# Нормирование операции АБР

{% hint style="info" %}
Выполняется для подразделения АБР ЛМО
{% endhint %}

## Расчет доп. характеристик

### R19 - Количество секций

Данные берутся из доп. характеристик KSM

## Расчет норм

### Расчет нормы S20 - Операционные нормы использования оборудования

?????

### Расчет нормы S21 - Операционные нормы времени и расценки

S21 = ((ttmrUsed  Math.Abs(r25) / koid + (ttmrRec.Ttmr1  Math.Abs(r19)) / obpart)  Math.Abs(r20))  kolrab  koefsht, где:

r19 - Количество секций радиатора;

Остальное аналогично [общему расчету S21](raschet-norm-s21.md)
