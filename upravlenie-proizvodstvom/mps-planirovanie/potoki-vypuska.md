---
description: Инструкция по планированию потоков выпуска
---

# Потоки выпуска

{% hint style="info" %}
Управление производством → Управление производством и загрузкой мощностей → Планирование → MPS, MRP-планирование
{% endhint %}

![](<../../.gitbook/assets/0 (132).png>)

Для работы с MPS планом

**Имеется следующие пункты меню (вызов по F2)**

![](<../../.gitbook/assets/1 (132).png>)

**Обычно приоритеты проставляю в конце месяца на следующий месяц.**

Все три кнопки работают по одному принципу и делают одно и то же

\- **Проставить приоритет для G0102** проставляет приоритет для Потока 1 и Потока 2 сразу

\- **Проставить приоритет для G0102 Поток 1 соответственно** проставляет приоритет только для Потока 1

\- **Проставить приоритет для G0102 Поток 2 соответственно** проставляет приоритет только для Потока 2

Отбор и простановка происходит по следующим правилам:

Для Leas 1 6250 штук в неделю

Для Leas 2 7500 штук в неделю

Процесс распределения дат приоритетов (расстановка) ВСЕГДА начинается с ближайшей пятницы

Не посредственно расстановка приоритетов происходит по сложным правилам описанным в таблице Prior\_, таким образом чтобы время перенастройки было минимальным.

В Отбор попадают (для простановки дат и приоритетов) попадают записи отвечающие следующим условиям:

\- ресурсы группы G0102

\- Строки PLA имеют приоритет (Больше 100 и меньше 900) или 0 (т.е. приоритет еще не проставлялся

\- Статус Утвержден (Поле KSTATUS=’3’)

**Для примера**

![](<../../.gitbook/assets/2 (134).png>)

![](<../../.gitbook/assets/3 (41).png>)

**Такой заказ будет участвовать в распределении приоритетов и дат, потому что**

**Группа G0102, приоритет 118 (Это больше 100, но меньше 900), статус заказа утвержден**

**А Вот такой:**

![](<../../.gitbook/assets/4 (98).png>)

**Не будет потому что приоритет 99 (Менее 100)**

По Сути приоритеты в области о 1 до 99 проставляются вручную и используются для самых приоритетных задач, а приоритеты больше 900 наоборот для менее приоритетных
