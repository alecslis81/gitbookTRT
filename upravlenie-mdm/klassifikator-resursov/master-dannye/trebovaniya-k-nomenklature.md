---
description: >-
  Требования к заведению ресурсов в справочник номенклатуры мастер данных
  (базовые данные для всех площадок)
---

# Требования к номенклатуре (мастер данные)

**Заполняемые данные по закладкам**

![](<../../../.gitbook/assets/image (525).png>)

**РЕСУРС**

* Обозначение
* Наименование (обязательно для всех ресурсов)
* Учетная ЕИ
  * Учетная ЕИ - учетная единица измерения
  * ЕИ-2 - используется для перевода в учетную единицу измерения
  * ЕИ-3 - используется для перевода в учетную единицу измерения
  * ЕИ-нормМ - единица измерения используется при нормировании
  * ЕИ-кальк - единица измерения используется при калькулировании
  * ЕИ-нормП - единица измерения используется при планировании
* ГОСТ, ТУ, ...

**КОНСТРУКТОРСКИЕ ПРИЗНАКИ**

* Признак изготовления (обязательно для всех ресурсов)
* Раздел КС
* Плотность (для материалов группы М)
* Габариты: ДхШхВхД

**ПРОИЗВОДСТВО**

* Подразделение (для номенклатуры собственного производства). Применяется при формировании [плана производства](../../../upravlenie-proizvodstvom/mps-planirovanie/mps-plan/formirovanie-plana-proizvodstva.md) и при расчете [потребности под задания](../../../upravlenie-proizvodstvom/proizvodstvennye-zadaniya/raschet-potrebnosti-v-materialakh-pod-zadanie.md)

**ЗАКУПКИ**

* Оперативная группа (для номенклатуры с признаком закупка)
* Основной склад (НЕ ЗАПОЛНЯТЬ - вместо этого необходимо вести [Справочник складов для приходования](../../../upravlenie-zakupkami/nsi/spravochnik-skladov-dlya-prikhodovaniya.md))
* Цикл закупки (дней) и Мин.партия (кратность) (НЕ ЗАПОЛНЯТЬ - вместо этого необходимо вести справочник [Циклы и кратности](../../../upravlenie-zakupkami/nsi/cikly-i-kratnosti.md))
* % толеранса - заполнять для номенклатуры с признаком закупка и имеющий допуск в поставке. Применяется в процессе [Формирования прихода по графику поставки](../../../uchet/postuplenie-tovarov-i-uslug/formirovanie-prikhoda-po-grafiku-postavki/)
* ABC класс - используется при списании номенклатуры группы "С"

**ЭКОНОМИКА**

* Тип ресурса (обязательно для всех ресурсов)
* План счетов (обязательно для всех ресурсов)
* Счет хранения (обязательно для всех ресурсов)
* Тип начисления НДС (обязательно для номенклатуры с признаком закупка)

**КОДЫ**

* Код ЕС НСИ (заполняется для номенклатуры группу G обязательно, для остальных ресурсов по потребности)

**ДОПОЛНИТЕЛЬНО**

* Доп.признак 1 - Заполняется автоматически при аннулировании документации (КД)
* Доп.признак 2 - Заполняется для номенклатуры группы G, являющейся продукцией
* Доп.признак 3 - Заполняется для номенклатуры которую необходимо выдавать в эксплуатацию
* Извещение - Заполняется автоматически при создании ресурса по извещению

**ДОП.ХАРАКТЕРИСТИКИ**

Заполняется автоматически на основании данных ЕС НСИ

## Правила заполнения

* Обращать внимание на указание группы ресурсов и тип ресурса

| **Группа** | **Наименование**                    | **Тип ресурса**                                                                                                              |
| ---------- | ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| G          | Готовая продукция                   |  ПродукцияГотовая                                                                                                            |
| Г          | Изделия по ГОСТам                   | <p>ПокупныеИзделия</p><p> (Г50 – ИнструментТехоснастк)</p>                                                                   |
| Д          | Нормативно-техническая документация |  Не проставляем                                                                                                              |
| И          | Инструмент                          | ИнструментТехоснастк                                                                                                         |
| К          | Комплектующие                       | <p>ПокупныеИзделия</p><p>К50 – Упаковка</p><p>К14 – Оборудование</p><p>К17 - Материалы</p>                                   |
| М          | Материалы                           | <p>Материалы</p><p>М00 – ВозвратныеОтходы</p><p>М40 – ЧерныйМеталл</p><p> (кроме М4007, М40А0, М40А1 - НержавеющаяСталь)</p> |
| О          | Оборудование                        | <p>Оборудование</p><p>О18 – ИнструментТехоснастк</p>                                                                         |
| П          | ДСЕ продукции                       | <p>Полуфабрикаты</p><p>Упаковка</p><p>Покупные изделия (ФР-ресурсы по чертежам)</p>                                          |
| У          | Услуги                              | Услуги                                                                                                                       |

* Единицы измерения (в каких ЕИ поставляется ресурс, объемы тары)

Список групп, для которых обязательно заведение второй ЕИ: Г (Из ШТ в КГ)

* Счет хранения (для канцтоваров уточнить у Фроленко Марина Владиславовна)

| **Группа** | **Наименование**            | **Счет хранения**                      | **Наименование**                                                               |
| ---------- | --------------------------- | -------------------------------------- | ------------------------------------------------------------------------------ |
| G          | Готовая продукция           | 43.01                                  |                                                                                |
| Г          | Изделия по ГОСТам           | 10.02                                  | Покупные п/фабрикаты и комплектующие изделия                                   |
| Д          | Нормативно-техническая док. | -                                      |                                                                                |
| И          | Инструмент                  | 10.09                                  | Инвентарь и хозяйственные принадлежности                                       |
| К          | Комплектующие               | <p>10.02</p><p>(Кроме К14 – 10.05)</p> | <p>Покупные п/фабрикаты и комплектующие изделия</p><p>К14 - Запасные части</p> |
| М          | Материалы                   | 10.01                                  | Сырье и материалы                                                              |
| О          | Оборудование                | 10.05                                  | Запасные части                                                                 |
| П          | ДСЕ продукции               | <p>20.011</p><p>10.02</p>              | <p>Полуфабрикаты собственного производства</p><p>Покупные изделия</p>          |
| У          | Услуги                      | 10.07.2                                | ДСЕ, переданные в переработку на сторону                                       |
