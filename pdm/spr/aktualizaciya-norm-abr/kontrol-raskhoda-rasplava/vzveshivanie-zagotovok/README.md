---
description: >-
  Инструкция по внесению фактических данных взвешивания секций, коллекторов и
  литников
---

# Взвешивание заготовок

{% hint style="info" %}
Логистика → Управление документооборотом материальных и финансовых потоков → Взвешивание → Контроль расхода расплава
{% endhint %}

## Добавление заголовка

Для добавления новых данных нажмите на кнопку «Добавить» и заполните обязательные строки

![
](<../../../../../.gitbook/assets/0 (29)>)

* Рабочий центр - Рабочий центр с которого взвешиваю заготовку
* Карта раскроя - Пресс-форма
* Количество потоков - Количество гнезд в пресс-форме
* Вес литника - Вес литника, кг

![](<../../../../../.gitbook/assets/0 (14)>)

* **Вес литника превышает норму**\
  Данный показатель будет отмечен если фактический вес литника будет превышать норму, установленную на литник
* **Вес секции превышает норму**\
  Данный показатель будет отмечен если хотя бы один фактический средний вес расплава (по ресурсу) будет превышать норму, установленную на расплав.\
  Более подробно можно рассмотреть в строках

По окончанию внесения взвешивания необходимо передать документ по бизнес-процессу

## Добавление строк

{% hint style="info" %}
Красный цвет означает, что не сформированы строки взвешивания
{% endhint %}

![](<../../../../../.gitbook/assets/1 (30)>)

Чтобы сформировать строки необходимо вызвать режим Сформировать строки взвешивания (F2 -> Сформировать строки взвешивания)

![](<../../../../../.gitbook/assets/image (203).png>)

Необходимо заполнить:

* Вес секций, кг
* Вес коллектора, кг (для биметаллических секций)



![](<../../../../../.gitbook/assets/1 (43)>)

* **Вес**\
  Значение установленной нормы
*   **Отклонение**

    * **Литник**

    Разница между **Литник (на секцию)** и **Норма Литник Вес (на секцию).**\
    Показатель **Отклонение** будет **красным** если фактический вес **( Литник (на секцию) )** больше, чем нормативный ( **Норма Литник Вес (на секцию) )**

    * **Расплав**

    Разница между **Вес** **Расплав** и **Норма Расплав Вес**\
    Показатель **Отклонение** будет **красным** если фактический вес **( Вес** **Расплав )** больше, чем нормативный ( **Норма Расплав Вес ).**

## Режимы F12

* Анализ норм (с заголовка взвешивания)
* Перейти к техмаршруту карты раскроя (с заголовка взвешивания)
* Перейти к спецификации (со строки взвешивания)
* Перейти к техмаршруту (со строки взвешивания)

## Режимы F2

* Удаление строк взвешивания (с заголовка взвешивания)

Чтобы отредактировать взвешивание необходимо удалить строки взвешивания (режим доступен до стадии «Анализ»)

![](<../../../../../.gitbook/assets/0 (48)>)