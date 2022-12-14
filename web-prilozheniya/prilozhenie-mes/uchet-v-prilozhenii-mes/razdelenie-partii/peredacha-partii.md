---
description: Инструкция по формированию передачи, подтверждения и отмены партии ТМЦ
---

# Передача партии

## Передача партии

Функцию использовать для формирования документа перемещения партии. Формируется документ [Внутреннее перемещение](../../../../uchet/peremesheniya-tovarov-1/vnutrennee-peremeshenie/)

![](<../../../../.gitbook/assets/0 (7)>)

Для передачи на форме сначала надо выбрать соответствующее действие, Передать партию

Затем сканируется или вводится штрих-код партии, автоматически запрашивается информация по ней. Текущее количество отображается в поле и не подлежит редактированию, т.к. партия передается только полностью

После этого надо выбрать из списка [подразделение-получатель](../../../../upravlenie-mdm/spravochnik-podrazdelenii/podrazdeleniya.md)

{% hint style="info" %}
Подразделения выбираются по условию:

* не отмененное
* Учетная точка
{% endhint %}

По нажатию на кнопку «Передать партию» будет создан документ [внутреннего перемещения](../../../../uchet/peremesheniya-tovarov-1/vnutrennee-peremeshenie/) партии между подразделениями

{% hint style="info" %}
Партия при перемещении не меняется
{% endhint %}

## Приемка партии

Функцию использовать для подтверждения приемки партии

![](<../../../../.gitbook/assets/image (279).png>)

Сканируется или вводится вручную штрих-код партии, которую надо принять

{% hint style="info" %}
По партии система ищет документ [внутреннее перемещение](../../../../uchet/peremesheniya-tovarov-1/vnutrennee-peremeshenie/) на стадии бизнес-процесса Подтверждение
{% endhint %}

Если партия найдена в документе отобразятся Данные о партии

![](<../../../../.gitbook/assets/image (728).png>)

{% hint style="info" %}
Если документ не найден или находится не на стадии Подтверждения, об этом будет указано в поле
{% endhint %}

![](<../../../../.gitbook/assets/image (242).png>)

Ввод количества при подтверждении не требуется

При нажатии кнопки «Принять партию» проверяется наличие прав у пользователя на это действие. Права на подтверждение по подразделениям прописываются в справочнике [MES.Справочник ответственных для приемки](../../../../uchet/nsi-uchet/spravochniki-pravil-peremesheniya.md#mes.-spravochnik-otvetstvennykh-dlya-priemki)

Если у пользователя есть права на подтверждение, документ передается далее по бизнес-процессу

## Возврат партии

Функцию использовать в случае отмены приемки партии

![](<../../../../.gitbook/assets/image (140).png>)

Сканируется или вводится вручную штрих-код партии, которую надо принять, автоматически запрашивается документ внутреннего перемещения по этой партии

{% hint style="info" %}
Документ должен находиться на стадии БП [Подтверждение](../../../../uchet/peremesheniya-tovarov-1/biznes-processy-peremesheniya/bp.vnutrenee-peremeshenie.md)
{% endhint %}

Если документ найдет корректно, данные о партии отобразятся в поле

![](<../../../../.gitbook/assets/image (508).png>)

Если документ не найден или находится не на стадии Подтверждения, об этом будет указано в поле

![](<../../../../.gitbook/assets/image (181).png>)

Ввод количества при возврате не требуется

При нажатии кнопки «Вернуть партию» проверяется наличие прав у пользователя на это действие. Права на возврат по подразделениям прописываются в интерфейсе

{% hint style="info" %}
Если у пользователя есть права на возврат, документ внутреннего перемещения отменяется
{% endhint %}
