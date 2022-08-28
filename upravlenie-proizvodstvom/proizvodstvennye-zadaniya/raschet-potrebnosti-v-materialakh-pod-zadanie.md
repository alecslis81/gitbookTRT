---
description: Инструкция по расчету потребности в материалах под производственные задания
---

# Расчет потребности в материалах

## Бизнес объекты

{% hint style="info" %}
В расчет попадает номенклатура по условию в бизнес-объекте BR.MP.SFC.ST.MD.MC
{% endhint %}

Пример по РТ

(KSKL > 0 or CEH\_N > 0 or ksp1='1') and KKS2<>'1'

Попадают позиции у которых в справочнике ресурсов заполнено хотя бы одно из полей:

* KSKL - Основной склад хранения. Код
* CEH\_N - Основное подразделение. Код
* ksp1 = 1 - Признак изготовления равен "Покупные"
* KKS2<>'1' - Дополнительный признак 2 не равен "Изделие"

## Расчет потребности

Для того что бы рассчитать потребность необходимо с заголовка задания запустить расчет Дефицита материалов и комплектующих (F2 - Обеспечение материалами - Расчет дефицита материалов и комплектующих)&#x20;

![](<../../.gitbook/assets/image (288).png>)

* Расчет дефицита материалов и комплектующих - Режим при котором система спросит формировать или нет Заявку на выдачу дефицитных материалов. Расчет происходит с учетом прав пользователей
* Передать заявку на выдачу материалов - Передача [Заявки на выдачу](zayavka-na-vydachu-materialov-1.md) вперед по Бизнес процессу
* Расчет дефицита материалов и комплектующих (авто) - Автоматически рассчитывает дефицит и формирует заявку на выдачу. Расчет происходит на сервере с правами Робота

Результаты расчетов можно посмотреть на закладке Материалы

![](<../../.gitbook/assets/image (292).png>)

Если заявка на выдачу не была сформирована в момент расчета дефицита ее можно вызвать отдельным режимом (F2 - Вызов формирования заявок)

![](<../../.gitbook/assets/image (324).png>)

{% hint style="info" %}
Заявка может быть сформирована только на строку с признаком покупка и у которых определен основной склад хранения
{% endhint %}

После формирования заявки для дальнейшей работы с ней необходимо перейти к документы (F12 - Перейти к заявке на выдачу)

![](<../../.gitbook/assets/image (986).png>)

## Склады хранения

Правила определяется:

* Основной склад в [корпоративном классификаторе](../../upravlenie-mdm/klassifikator-resursov/master-dannye/trebovaniya-k-nomenklature-dannye-ploshadok.md) по объекту (KSMO.KSKL)
* [Склады хранения ресурсов по подразделениям](../../upravlenie-zakupkami/nsi/spravochnik-skladov-dlya-prikhodovaniya.md) (PWFD.CEH\_S) в связке с площадкой подразделения производственного задания
* Для ИЗТТ по умолчанию, если не указана информация по пунктам выше, по площадке Киржач - Склад ОП г. Киржач, Ижевск - Склад ПКИ Гагарина 1

Комментарий:

* SOS склад - если у ресурса Призн. изготовления (KSM.KSP1) "1 (Покупные)" и не указан основной склад хранения
* SOS abc - если Потребность нетто более остатка и ресурс из группы "C" ABC классификатора
* SOS норм.спис. - если Потребность нетто более остатка и ресурс из группы справочника нормативного списания

![](<../../.gitbook/assets/image (65).png>)

## Методы

Проставить признак ABC - проставляет в KSMO признак С

![](<../../.gitbook/assets/image (574).png>)
