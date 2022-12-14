# Сходимость УМО

{% hint style="info" %}
Управление производством → Управление производством и загрузкой мощностей (MRPII) → Анализ → Сходимость линий УМО
{% endhint %}

Предназначен для контроля выработки, установленных секций на линиях УМО.

При запуске выбираем параметры отчета\
![](<../../../../.gitbook/assets/0 (37)>)

Отчет представлен в виде иерархии, которая построена на 3 уровнях\
Дата -> РЦ-> Партия

![](<../../../../.gitbook/assets/1 (27)>)

**Основные данные:**

* **Дата** – дата выработки РЦ ЛМО
* **Модель** – под ней подразумевается, модель, код, штрих-код, партия
* **ФИО** – ФИО сотрудника зарегистрировавший выработку
* **Секции –** секции выпускаемого радиатора
* **Установка; Уст.сек –** установленные секции
* **Установка ;Исп. Сек –** использование установленных секции в производстве
* **Установка; Остаток** – **** отклонения между **(**Уст.сек - Исп.Сек)**.** Остаток установленных секций
* **Передача в оконч.брак –** Кол-во секций , переданных в окончательный брак
* **Вал потреб**.**секций** – Вал использованных секций
* **Выход**; **годные** – выход годных (радиаторов | секций)
* **Выход**; **Испр.брак** – выход исправимого брака (радиаторов | секций)
* **Выход**; **Вал.сек** – Валовый выход секций (годные + исправимый + передача в оконч. брак)
* **Отклонение** – (Вал потреб.секций - Выход;Вал.сек)
