---
description: Инструкция по корректировке входящих цен по процессу Приход по плановым ценам
---

# Внесение фактических цен

Формирование фактических расходов производим на основании документов прихода с учетом признака Цены ТМЦ:

* Плановые -> Фактические цены прихода / Дополнительные затраты
* Фактические -> Дополнительные затраты

## Формирование документа доп затрат на приход по плановым ценам

В момент поступления документ (УПД) от поставщика вносим в ИТЕ фактические цены через Документ ЦеныФакт (COM\_SUP\_V1). Для этого находим первоначальный документ Приход ТМЦ от поставщика, встаем на него и вызываем режим Добавить фактические цены прихода и доп. затраты (F2 ->  Добавить фактические цены прихода и доп. затраты):

![](<../../../.gitbook/assets/image (246).png>)

Появляется документ «Цены факт» - устанавливаем дату документа не позднее последнего дня календарного месяца, в котором была поставка ТМЦ.

![](<../../../.gitbook/assets/15 (6).png>)

Открываем строчную ( табличную) часть документа – заполняем фактическую цену из документа ( УПД, накладная), сумма пересчитывается автоматически.

Нажимаем кнопку «Сохранить»

![](<../../../.gitbook/assets/16 (6).png>)

Проверяем строчную часть документа – должна появиться сумма в колонке «Разница».

Проводки ДТ 10.01, 10.02 Кт 60

Передаем документ вперед ( зеленая стрелка в правом углу).

![](<../../../.gitbook/assets/17 (5).png>)

Меняется Стадия документа Ввод – Проводки

В поле экрана Реестр документов в колонке Б появился +

{% hint style="info" %}
Если после формирования приходных документов появляются дополнительные услуги, то в строчной части документа нажимаем клавишу F7 «Добавить» и выбираем вид дополнительных расходов (Таможенный сбор; Пошлина; Страхование; ТЗР прочих контрагентов)
{% endhint %}

## Формирование документа доп затрат на приход по фактическим ценам

Создается документ ДопЗатраты (COM\_SUP\_V5), в котором закрыто редактирование цены и суммы для строк ТМЦ, возможно только добавление строк услуг

## Внесение дополнительный услуг

Дополнительные услуги заполняем аналогично [Приходу ТМЦ в валюте](prikhod-tmc-ot-postavshika-valyuta-import/)
