---
description: Инструкция по анализу выработки участков Термокомпонента
---

# Монитор выработки ТК

{% hint style="info" %}
Отчеты → Мониторы → TK → Монитор выработки
{% endhint %}

При запуске монитор формирует данные за текущий день.

Внешний вид монитора

![](<../../../../.gitbook/assets/0 (77)>)

Вкладки:

* Резка
* Трансфера
* Сварка

В зависимости от вкладки формируется, соответствующий отчет

Данные монитора:

1. **№,** номер РЦ
2. **СМ,** номер смены
3. **Наименование РЦ,** название оборудования
4. **Цикл,** средний цикл выпускаемых изделий, рабочим центром
5. **Прошло часов, с**колько часов прошло с момента начала смены
6. **Норматив; за см шт,** норматив выпуска за смену
7. **Норматив; за часы работы шт,** норматив выпуска за прошедшее время от начала смены
8. **Выпуск; Факт вып. шт ,** фактический выпуск по РЦ
9. **Выпуск; IIOT,** выпуск по датчикам IIOT
10. **Откл,** отклонение между **Выпуск; Факт вып. шт** и **Норматив; за часы работы шт**
11. **% Выработки,** отношение **Выпуск; Факт вып. шт** и **Норматив; за часы работы шт**
12. **% Производительности,** отношение **Выпуск; Факт вып. шт** и **Норматив; за см шт**
13. **Норма / час,** норма выпуска продукции за 1 час
14. **Почасовая выработка,** выработка за каждый час
