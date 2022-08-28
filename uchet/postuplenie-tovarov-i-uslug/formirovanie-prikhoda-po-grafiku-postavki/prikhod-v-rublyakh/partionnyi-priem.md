---
description: Инструкция по партионной приемке матриалов
---

# Партионный прием

## Создание поступления

Формирование документа поступления выполняется менеджером по [инструкции ](../)

{% hint style="info" %}
Заводится одна строка с суммарным количеством по документу прихода
{% endhint %}

## Партионная приемка

Документ передается на стадию [приемка товара](../../biznes-processy-prikhoda/). На стадии сотрудник производит контроль количества и формирование партий прихода

{% hint style="info" %}
Логистика → Управление документооборотом материальных и финансовых потоков → Взвешивание → Приход ТМЦ
{% endhint %}

![](<../../../../.gitbook/assets/0 (86).png>)

### Добавление партии прихода

* Вес партии фиксируется автоматически (на РТ) или руками

При приходовании автоматически фиксируется отклонение от планового количества

![](<../../../../.gitbook/assets/1 (76).png>)

После завершение взвешивания документ передается на следующую стадию

![](<../../../../.gitbook/assets/2 (66).png>)

### Характеристики партии

Для части номенклатуры необходимо дополнительно вносить характеристики партии:

* Номер плавки - номер плавки с сертификата качества

Номер плавки обязательно к заполнению если для ресурса применяется [характеристика качества](../../../../upravlenie-kachestvom/nsi/kharakteristiki-kachestva/) (код характеристики 8355)

* Количество - количество единиц продукции в партии

Количество обязательно к заполнению если ресурс есть в [справочнике расчета фактических норм по партиям поставщика](../../../dokumenty-vyrabotki/uchet-po-vesu-partii/uchet-po-vesu-partii-na-tk/spravochnik-raschet-fakt-norm.md)

![](<../../../../.gitbook/assets/image (971).png>)

### Журнал входного контроля

{% hint style="info" %}
Журнал входного контроля формируется в разрезе партий приемки
{% endhint %}

![](<../../../../.gitbook/assets/3 (70).png>)

## Режимы

### Перейти к взвешиванию и нормам (F12)

По сохраненным взвешиваниям создаются строки с фактическими партиями, и при необходимости рассчитываются нормы фактического списания. Режим позволяет просмотреть нормы по каждой партии (работает в т.ч. при множественном выборе строк)

### Заполнить количество единиц по партии прихода (F2)

Режим используется для заполнения нормы для принятых ранее партий