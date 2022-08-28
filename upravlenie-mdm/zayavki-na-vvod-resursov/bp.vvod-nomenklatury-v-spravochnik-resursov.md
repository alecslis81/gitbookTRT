---
description: Описание бизнес-процесса по вводу и корректировке НСИ
---

# Бизнес-процессы по НСИ

![](<../../.gitbook/assets/image (470).png>)

| Стадия          | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Заявка          | <p><strong>Инициатором заявки является пользователь.</strong></p><p>Пользователь вводит заголовок извещения на изменение классификатора ресурсов.</p><p>Введенному извещению автоматически присваивается стадия <strong>«Заявка».</strong></p><p>Пользователь вводит в извещение строки типа <strong>«Добавление»</strong> с указанием группы, в которую необходимо добавить новый ресурс, и обязательного перечня реквизитов ресурса. Либо строки типа <strong>«Удалить»</strong> или <strong>«Изменить»</strong> с указанием кода ресурса, который необходимо изменить/удалить.</p><p>После ввода всех строк – передает извещение вперед по маршруту стадийной обработки для согласования и проведения</p> |
| Возможные дубли | <p>Автоматическая проверка системой, на возможные дубли.</p><p>При обнаружении возможных дублей система предложит выбрать уже существующий ресурс.</p><p>Если в заявке присутствуют строки только на добавление ресурсов, и для каждой из них применен предложенный ресурс из возможных дубликатов, заявка пойдет на стадию выгрузки в 1С</p><p>Во всех остальных случаях потребуется согласование специалистов НСИ</p>                                                                                                                                                                                                                                                                                      |
| Проверка        | <p>Проверка на добавление новой записи или изменение <strong>наименования</strong> принадлежит специалисту <strong>НСИ</strong></p><p>Извещение переводится на стадию <strong>«Проверка»</strong>, на которой</p><p>исполнитель, ответственный за добавление записей в классификатор ресурсов, принимает решение о добавлении нового кода ресурса в классификатор путем передачи извещения вперед по маршруту стадийности, или об отклонении извещения (например, по причине не верно выбранной группы) путем его возврата на предыдущую стадию с обязательным указанием в резолюции причины, по которой извещение отклонено.</p>                                                                            |
| Проведение      | Ответственный исполнитель вызывает расчет **«Провести извещение в классификаторе ресурсов»**, после успешного проведения которого в классификатор добавляется новый ресурс, а извещение переводится на стадию **«Выгрузка в 1С»**                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Выгрузка в 1С   | Из функционала планировщика задач системы **«IT-Enterprise»** запускается расчет, по которому автоматически выгружаются все извещения, находящиеся на стадии **«Выгрузка в 1С»** и переводятся на стадию **«Импорт из 1С»**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Импорт из 1С    | На стадии **«Импорт из 1С»** ожидается ответный пакет от системы 1С об окончании успешной обработки выгруженных данных в 1С                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ЕС НСИ          | [Импорт данных из ЕС НСИ](../../integraciya/integraciya-s-es-nsi.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Архив           | Ресурс синхронизирован по всем БД, заявка переводится на стадию «Архив»                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

Инструкции -> [Заявки на ввод ресурсов](./)