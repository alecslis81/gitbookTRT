---
description: Инструкция по формированию документов Акт выполненных работ
---

# Акт выполненных работ

Документ передача товаров создается по документам «Передача товаров в переработку» в разрезе организации, договора, заказа.

{% hint style="info" %}
Если по документу есть акт выполненных работ, то повторно по документу акт выполненных работ **НЕ ФОРМИРУЕТСЯ**
{% endhint %}

Зайдите в реестр документов. Встаньте курсором на документ «Передача товаров из переработки» и нажмите «F2 – Создание акта выполненных работ переработка»:

![](<../../../.gitbook/assets/0 (123).png>)

В появившемся окне заполните все поля и нажмите «ОК»:

![](<../../../.gitbook/assets/1 (36).png>)

* «Дата с:» - «Дата по:» - период, за который формируется акт выполненных работ
* «Организация» - по умолчанию из документа «Передача товаров в переработку»
* «Договор» - по умолчанию из документа «Передача товаров в переработку»
* «Заказ» - для выбора предлагается список заказов с типом «заказ на услугу», созданный для указанной организации

По окончании создания акта выполненных работ на экране появится окно:

![](<../../../.gitbook/assets/2 (31).png>)

Нажмите «Да» для просмотра документа:

![](<../../../.gitbook/assets/3 (19).png>)

Документ создается на стадии «Ввод».

Переведите документ на следующую стадию «Экспорт 1С», нажав кнопку «Передать вперед»:

![](<../../../.gitbook/assets/4 (45).png>)

На стадии «Экспорт 1С» автоматически создается пакет для экспорта в 1С

Когда пакет создан и отправлен в 1, документ АВТОМАТИЧЕСКИ переходит на стадию «импорт 1С»

Когда из 1С приходит ответ с номером документа в 1С и ответ загружается в систему It – Interprise, документ АВТОМАТИЧЕСКИ переходит на стадию «Архив»
