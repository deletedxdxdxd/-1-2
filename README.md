Fitness Center API — Отчёт 1 (in-memory)
REST API для управления фитнес-центром. Данные хранятся в памяти процесса (in-memory, Map).
Во второй части хранилище заменяется на реальную СУБД без изменения контроллеров и маршрутов.
| Компоненты | Решение |
| ------------- | ------------- |
| Язык | C# |
| Хранилище | In-memory (Map) |
| First Header | Second Header |
| ------------- | ------------- |
| Content Cell | Content Cell |
| Content Cell | Content Cell |

Модели данных
Client
Поле | Тип	Обязательно |	Описание
id |	UUID | генерируется | Уникальный | идентификатор
surname |	String | ✅ | Фамилия
name | String | ✅|	Имя
patronymic | String | ❌ | 	Отчество (null если не указано)
birthday | Date | ✅ | Дата рождения (YYYY-MM-DD)
phone | String | ✅ |Номер телефона
email | String | ✅ | Email
is_active | Boolean | по умолч. true | Активен ли клиент
trainer_id | UUID | ❌ | Ссылка на тренера
