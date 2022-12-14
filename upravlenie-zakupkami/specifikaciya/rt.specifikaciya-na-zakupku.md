---
description: >-
  Дополнительная инструкция для Royal Thermo по формированию и согласованию
  спецификаций
---

# РТ.Спецификация на закупку

**Вид отображения Спецификации на закупку ТМЦ**

{% hint style="info" %}
Реестр документов → Поступление товаров и услуг → Спецификация на закупку
{% endhint %}

Служебные стадии наполнения и контроля Коммерческим отделом:

* Инициатор
* Проверка ДСП
* Формирование графика поставки
* Расчет аналитик по цене
* Руководитель подразделения

## **Наполнение Спецификаций на стадии Инициатор**

Заголовок Спецификации должен быть заполнен в соответствии с данными документа основания закупки (те в соответствии с вложенными счетом или спецификацией поставщика, а также с условиями договора).

### **Вкладка Документ**

на данной вкладке должны быть заполнены данные:

* Наименование контрагента
* Выбран договор для Спецификаций:

{% hint style="info" %}
с суммой свыше 42 000 руб. с НДС, наличие договора обязательно, договор должен быть подписан и находится в Архиве, в противном случае оплата невозможна
{% endhint %}

{% hint style="info" %}
с суммой менее, 42 000 руб. с НДС, наличие договора не является обязательным, но принято и системно установлено ограничение: сумма всех созданных и незакрытых поставкой Спецификаций по одному поставщику не должно превышать установленную сумму
{% endhint %}

{% hint style="info" %}
с Типом Счет-договор обязательно наличие правильно оформленного Счета-договора, согласно Инструкции от Симонова П.Е., а также принято и системно установлено ограничение: 1. не более 3-х Спецификаций от одного Поставщика; 2. Сумма по каждой Спецификации не должна превышать 500 000,00 руб. с НДС; 3. Сумма по всем неисполненным Спецификациям не должна превышать 500 000,00 руб. с НДС
{% endhint %}

* Валюта
* Проверена сумма закупки и сумма НДС
* Выбран Тип спецификации:

{% hint style="info" %}
Счет на оплату – простой Счет на оплату, в данном случае обязательно наличие Договора с поставщиком, либо сумма Счета не должна превышать 42 000 руб. с НДС
{% endhint %}

{% hint style="info" %}
Счет-договор – отдельный вид Счета с обязательными условиями, согласно Инструкции от Симонова П.Е.
{% endhint %}

{% hint style="info" %}
Юридическая спецификация – документ закупки, требующий подписания с двух сторон, наличие договора при этом обязательно
{% endhint %}

* Площадка: АБР либо СПР

![](<../../.gitbook/assets/image (775).png>)

### **Вкладка Дополнительно**

на данной вкладке должны быть заполнены данные:

* Инициатор закупки

![](<../../.gitbook/assets/image (143).png>)

### **Вкладка Способ доставки**

на данной вкладке должны быть заполнены данные:

* Условия поставки

![](<../../.gitbook/assets/image (8).png>)

### **Вкладка Документы**

на данной вкладке должны быть заполнены данные:

* № и дата документа-основания закупки: Спецификации или Счета
* Условия продажи
* Условия оплаты и поставки

![](<../../.gitbook/assets/image (117).png>)

## **Заполнение условий оплаты и поставки**

### Проверка условий по договору

На заголовке Спецификации F12 -> Карточка договора

![](<../../.gitbook/assets/image (797).png>)

Открываем договор (под скрепкой) и читаем пункты, где прописаны Условия оплаты и Условия поставки

![](<../../.gitbook/assets/image (291).png>)

Условия в карточке Спецификации должны полностью соответствовать условиям оплаты по Договору, либо соответствовать условиям оплаты документа-основания закупки, если в договоре указано, что условия оплаты и поставки определяются на каждую поставку отдельно в документе-основания закупки

![](<../../.gitbook/assets/image (14).png>)

Проверка условий оплаты: Логистика → Управление документооборотом материальных и финансовых потоков → Настройка → Справочники к документам движения → Условия оплаты

![](<../../.gitbook/assets/image (792).png>)

Фильтруем по коду, указанному в Спецификации, и проверяем условия заполнения строк:

* Тип платежа: Постоплата или Предоплата
* Дни: количество дней отсрочки оплаты в соответствии с условиями Договора
* Тип отсчета дней: Банковские или Календарные
* Тип события отсчета: Готовность (он же Отгрузка) или Приемка

## **Наполнение строк Спецификации позициями, закупаемых ТМЦ**:

* Наименование – должно соответствовать документу основанию закупки и внутреннему справочнику ресурсов ИТе
* Количество – в соответствии с документом основания закупки
* Цена – в соответствии с документом основания закупки
* Сумма – рассчитывается автоматически, должна соответствовать документу основанию закупки
* Технология – все закупаемые ТМЦ должны быть включены (+) в один или несколько справочников (за исключением хоз. и канцтоваров):
  * М – материалы, используется в технологическом процессе при выпуске продукции
  * О – оснастка, инструмент, используются при в технологическом процессе при выпуске продукции
  * ЕАМ – ресурсы, используемые при обслуживании оборудования
  * З – замены, используются для всех вышеперечисленных справочников
* Соответствие плановой цене. Отклонение допустимо на 5%
* В случае отклонения от плановой цены более чем на 5%, либо в случае отсутствия плановой цены в Спецификацию должно быть вложено минимум 3 альтернативных предложения

![](<../../.gitbook/assets/image (495).png>)

## Согласование спецификаций на стадии Утверждение в реестре

Окончательное согласование Спецификации осуществляется Акционером Тимошенко М.В. и происходит на этапе Утверждение в реестре.

По проверенным Спецификациям формируются Строки КП, по которым в свою очередь формируется Реестр на оплату и направляется Акционеру на согласование.

Только после получения согласования закупка может считаться согласованной и размещенной у поставщика. После согласования Реестра на оплату Спецификации, по которым Строки КП были включены в данный Реестр, проходят автоматизированное согласование и переходят на стадию Исполнение

## **Срочные закупки**

В случае если необходимо провести срочную закупку:

* Менеджер ответственный за закупку:
  * создает Спецификацию на закупку на основании сформированной потребности направляет на согласование по бизнес-процессу
  * контролирует этапность прохождения
  * проводит согласование ДСП, в случае если такое согласование необходимо
* Руководитель коммерческой службы:
  * подписывает документ основание закупки у уполномоченного Директора завода
  * подписанный документ передает на оплату Руководителю финансовой службы
* Менеджер финансовой службы:
  * вручную формирует Строки КП, обрабатывает
  * проводит оплату
  * проводит согласование в Реестре на оплату.

Дальнейшее согласование проходит в стандартном порядке.

## **Контроль исполнения Спецификации**

Менеджер ответственный за закупку контролирует процесс исполнения закупки по Спецификации.

В случае если Спецификация не прошла автоматически в Архив, Менеджер проверяет причины:

* если неисполнение находится в пределах установленного толеранса, то Менеджер вручную продвигает документ по бизнес-процессу до Архива (одно нажатие на зеленую стрелочку)
* если неисполнение связано с ненадлежащим исполнением свои обязательств поставщиком, то Менеджер ответственный за закупку связывается с представителем поставщика, добивается исполнения обязательств по поставке
* в случае если дальнейшее исполнения поставки по Спецификации невозможно по объективным причинам, то Менеджер ответственный за закупку:
  * добивается проведения возврата аванса от поставщика, если он был
  * добивается получения компенсаций за непоставленные в срок ТМЦ, согласно условиям договора поставки
  * вручную продвигает Спецификацию по бизнес-процессу до Архива (одно нажатие на зеленую стрелочку), после чего закроется График поставки и потребность в закупке отобразится в Плане закупок

![](<../../.gitbook/assets/image (1).png>)

**Отмена спецификаций**
-----------------------

В случае если Спецификацию необходимо полностью отменить. Вместе со Спецификаций произойдет отмена связанных и незакрытых Графиков поставок

![](<../../.gitbook/assets/image (159).png>)

\
Условия Счета-договора – прописаны в Инструкции от Симонова П.Е.
----------------------------------------------------------------

{% hint style="danger" %}
**ОБЯЗАТЕЛЬНЫЕ ТИПОВЫЕ УСЛОВИЯ СЧЕТА-ДОГОВОРА**
{% endhint %}

| №    |                                                                                                                                                                                                                                                                                                                                                                                                     |
| ---- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1.   | Предметом настоящего Счета-договора является поставка товарно-материальных ценностей (далее - "товар")                                                                                                                                                                                                                                                                                              |
| 2.   | Оплата настоящего Счета-договора означает согласие Покупателя со всеми условиями оплаты и поставки товара.                                                                                                                                                                                                                                                                                          |
| 3.   | Настоящий Счет-договор действителен в течение 10 (Десяти) рабочих дней с момента его направления Покупателю.                                                                                                                                                                                                                                                                                        |
| 3.1. | При отсутствии оплаты в указанный срок настоящий Счет-договор признается недействительным.                                                                                                                                                                                                                                                                                                          |
| 4.   | Покупатель не имеет права производить выборочную оплату позиций счета и требовать поставку товара по выбранным позициям.                                                                                                                                                                                                                                                                            |
| 5.   | <p>Условия оплаты:</p><p><em><strong>100% предоплата/частичная предоплата (в каждом конкретном случае заполняется по факту)</strong></em></p><p><em><strong>В случае 100% предоплаты Поставщик вправе не выполнять поставку товара до зачисления 100 % оплаты на расчетный счет.</strong></em></p>                                                                                                  |
| 6.   | <p>Условия доставки товара: <em><strong>Заполняется в каждом конкретном случае индивидуально (самовывоз нашими силами со склада Поставщика, доставка Поставщиком до нашего склада или склада нашего перевозчика).</strong></em><br> <em><strong>С ОБЯЗАТЕЛЬНЫМ УКАЗАНИЕМ АДРЕСА!!!!</strong></em></p>                                                                                               |
| 6.1. | В случае доставки товара силами Поставщика до склада Покупателя или иного адреса, указанного выше, стоимость доставки входит в стоимость Товара                                                                                                                                                                                                                                                     |
| 7.   | Срок поставки: _**Заполняется в каждом конкретном случае индивидуально (срок должен быть четко указан!!! Например, 3 (рабочих) дня с момента перечисления Покупателем предоплаты**_                                                                                                                                                                                                                 |
| 8.   | <p>В случае нарушения Поставщиком срока поставки, Покупатель вправе взыскать с Поставщика неустойку в размере 0,2% от стоимости несвоевременно поставленного товара за каждый день просрочки.</p><p>В случае нарушения Покупателем сроков оплаты Поставленного товара, Поставщик вправе взыскать с Покупателя неустойку в размере 0,2% от суммы несвоевременной оплаты за каждый день просрочки</p> |
| 9.   | Все споры в рамках исполнения настоящего счета-договора рассматриваются в Арбитражном суде по месту нахождения Истца.                                                                                                                                                                                                                                                                               |

{% hint style="danger" %}
ЗАПРЕЩАЕТСЯ заключение счета-договора без включения в него обязательных типовых условий
{% endhint %}

{% hint style="danger" %}
ЗАПРЕЩАЕТСЯ заключение счета-договора с какими-либо иными условиями в нем, кроме типовых
{% endhint %}

## Дополнительная аналитика

* Проанализировать объем и цены закупки за год, можно с помощью команды F12, в строках Спецификации

![](<../../.gitbook/assets/image (132).png>)

Сформировать отчет

![](<../../.gitbook/assets/image (781).png>)

Проверяем периодичность, средний объем закупки и цены закупок

* Проверить остатки можно через Оборотно-сальдовую ведомость по ТМЦ

Вид отображения: Логистика → Учет запасов (складской учет) → Документы → Оборотно-сальдовая по ТМЦ

&#x20; Откроется рабочая область, где необходимо проставить фильтры

![](<../../.gitbook/assets/image (161).png>)

*  Дата на текущий момент
* Проставить V Развернуть до документов
* Проставить V Только детальные строки
* Группы и фильтры ставим галочки
  * Подразделения
  * Классификатор ресурсов, тут же + вставляем код ТМЦ
  * Сформировать

Получаем отчет по количеству ТМЦ на начало задаваемого периода и на конец. И на каких участках / складах имеются остатки

![](<../../.gitbook/assets/image (496).png>)
