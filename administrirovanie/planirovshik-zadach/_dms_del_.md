# \_DMS\_DEL\_

{% hint style="info" %}
Количеством Включенных задач планировщика регулируем нагрузку на CPU и Диски. **За нагрузкой смотреть постоянно!!!**
{% endhint %}

**Очередь диска – 150-200, много, но еще приемлимо (пользователи не жалуются, система работает), CPU я держу не более 80%, а лучше 65-70%**

Включать одновременно лучше не нужно – с разнице хотя бы в секунд 20-30, забор там устроен так что вызовет дедлоки по \_DMS\_L\_ (для системы не критично, а роботы по тупят)

**Из наблюдений: в рабочее время 2-3 штуки больше не вариант, вечером и рано утром можно в 6-7 потоков**

{% hint style="danger" %}
Роботы \_DMS\_DEL\_\* - не должны работать параллельно с переиндексацией DMS (по ночам что-то там происходит) – будут сбои!!!
{% endhint %}
