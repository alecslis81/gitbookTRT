---
description: Инструкция по работе с типопредставителями для готовой продукции группы G01
---

# Типопредставители для ГП

{% hint style="info" %}
**«Основное исполнение» -** это нулевое исполнение группы номенклатуры

* Для стальных радиаторов не указываем длину и высоту
* Для алюминиевого радиатора не указываем количество секций
{% endhint %}

{% hint style="info" %}
**Типопредставители -** используются для формирования таблицы [исполнений у конструкторской спецификации](../../../pdm/pdm-kpp/konstruktorskaya-podgotovka-proizvodstva/formirovanie-ispolnenii.md)
{% endhint %}

**Добавление «ТИПОПРЕДСТАВИТЕЛЯ»**

В IT-enterprise находим вкладку «**ГРУППЫ ПОДГРУППЫ РЕСУРСОВ**» находим группу «**G Готовая продукция» --> «Подгруппа»,** далее встаем на нужную подгруппу.

![](<../../../.gitbook/assets/0 (80).png>)

По коду ресурса или по наименованию находим номенклатуру, для которой нужно добавить **«ТИПОПРЕДСТАВИТЕЛЯ».**

{% hint style="info" %}
Если в IT-enterprise не заведено данное исполнение, то через функциональную клавишу **F2**, выбираем расчет **”**[**ФОРМИРОВАНИЕ ПАЧКИ РЕСУРСОВ**](dobavlenie-gruppy-resursov.md)**”.** Только для номенклатуры группы G01
{% endhint %}

Или создаем по образцу номенклатуру основного исполнения:

![](<../../../.gitbook/assets/1 (78).png>)

## Ручное формирование типопредставителей (для любой номенклатуры группы G)

Встаем на ресурс и в правом углу нажимаем значок **«ТИПОПРЕДСТАВИТЕЛЯ»**

![](<../../../.gitbook/assets/2 (68).png>)

В новом окне нажимаем функциональную клавишу **F7** или значок **«ДОБАВИТЬ»**

![](<../../../.gitbook/assets/3 (67).png>)

Далее появится еще одно окно **«ДОБАВЛЕНИЕ ТИПОПРЕДСТАВИТЕЛЯ»,** проваливаемся в поле **«ТИП»**

![](<../../../.gitbook/assets/4 (61).png>)

Выбираем строку **«ОСНОВНОЕ ИСПОЛНЕНИЕ»** нажимаем значок **«ВЫБРАТЬ»**

![](<../../../.gitbook/assets/5 (76).png>)

В поле **«ТИПОПРЕДСТАВИТЕЛЬ»** прописываем код ресурса нулевого исполнения. Жмем **«ДОБАВИТЬ»**

![](<../../../.gitbook/assets/6 (46).png>)

Для выхода из основного окна нажимаем горячею клавишу **ESC.**

**«ТИПОПРЕДСТАВИТЕЛЬ»** добавлен!

## Заполнение режимом (только для номенклатуры групп G0101 и G0102)

Для вызова режима необходимо находится на основном исполнении (F2 -> Работа с типопредставителями). Система автоматически сформирует типопреставители по всей группе ресурсов

![](<../../../.gitbook/assets/image (786).png>)

## Проверка

Для проверки на добавление **«ТИПОПРЕДСТАВИТЕЛЯ»,** проваливаемся в номенклатуру, вкладка «**КОДЫ»**, видим:

**«Тип»** – Основное исполнение

«**Типопредставители текущего ресурса» -** Радиатор…

«**Типопредставитель (КОД)»** – Код ресурса нулевого исполнения

![](<../../../.gitbook/assets/7 (18).png>)
