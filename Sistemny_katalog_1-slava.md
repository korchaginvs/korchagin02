##### Системный каталог
###### Описание pg_class
Получил описание таблицы с помощью команды **\d pg_class**:
![avatar](https://sun9-23.userapi.com/impg/cL12nCZtjhp1RA8rsdC4lyWnHEsgGEDFgeti5Q/fgOEgcganS8.jpg?size=504x580&quality=96&sign=7aed6e602a1397878119b5453b206176&type=album)
###### Подробное описание pg_tables
Подробное описание pg_tables(команда **\d+ pg_tables**):
![avatar](https://sun9-48.userapi.com/impg/2UxncSnu0ny9C0Sl1Lt4SAXOoQhhrDTc0pFApA/xvhToPaPBDs.jpg?size=589x382&quality=96&sign=56f241eef0e1ba41261a5e8a716ccfda&type=album)
###### Полный список схем
Создал базу данных и временную таблицу в ней.Получил полный список схем в базе, включая системные:
![avatar](https://sun9-48.userapi.com/impg/SPpkVB7wqE4Q6f8rWtgFcizYAwnXoW5Y24il9w/-G1n3hx0sEI.jpg?size=537x469&quality=96&sign=53ef66b788704f68ed63e41543ed4d8e&type=album)
###### Список представлений в information_schema
Использовал шаблон **\dv information_schema.***:
![avatar](https://sun9-28.userapi.com/impg/oMCAUy86NXzudo7Asfgq74NRTtjauPjos18y1Q/V1yVH_4vNGg.jpg?size=559x562&quality=96&sign=ed4d4e568a519946ede0ba00d82a45d7&type=album)
######  Запросы к системному каталогу
Чтобы увидеть запросы, которые выполняют команды psql, включим переменную ECHO_HIDDEN:
=> \set ECHO_HIDDEN on
=> \d+ pg_views
![avatar](https://sun9-69.userapi.com/impg/inwqEBGxlyfqgbCSl8lAAd5jaXcMHhvQ7cMaZw/PQrhxWlRfpk.jpg?size=660x565&quality=96&sign=f30d2937050bf32fa0e82cdfc2696780&type=album)
=> \set ECHO_HIDDEN off

