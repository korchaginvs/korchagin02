#### Аутентификация
При подключении клиента сервер должен выполнить несколько задач.Во-первых, идентифицировать пользователя, то есть определить его имя. Для этого пользователь представляется, но указанное имя может отличаться от имени пользователя БД (например, если пользователь представляется своим именем в ОС).
В целях выполнения данной лр я создал суперпользователя kat:
![avatar](https://sun9-24.userapi.com/impg/Mg1ABDx3zMZcfAwwRmeLgX1F-2b8A_Q9i8sueg/M9j6mWiC1YI.jpg?size=619x135&quality=96&sign=9201715919e35b2ad8917220d9b14232&type=album)
Затем я сохранил файл pg_hba.conf, чтобы иметь возможность восстановить:
![avatar](https://sun9-west.userapi.com/sun9-4/s/v1/ig2/aLds1UWUfqzbkvWkHTSSTrrqKb0OUMSvl6i8O5J52anYPKUG-zwBkxE-DEbEXbv6RomFifm5sc7XZJcfykhhgM_8.jpg?size=677x32&quality=96&type=album)
Проверил содержимое pg_hba.conf(используя представление pg_hba_file_rules):
![avatar](https://sun9-10.userapi.com/impg/vupbUl0RSJudUqEKEnHUAbVnVX5Nud7OdA_ZVQ/RGb0KFI4Zrw.jpg?size=594x189&quality=96&sign=562641d0ade742f8cc0ca4a408636e7f&type=album)
Затем перезаписал pg_hba.conf с нуля:
![avatar](https://sun9-east.userapi.com/sun9-42/s/v1/ig2/KJyTY1Cb1O2W8qOVtwL-XiTqbqD39ePVAGjJEn1Ioh7rMcmjljaAhmS0TjgHrhjeBDYMTgSHFPRsNdsH6PwYxe6N.jpg?size=560x134&quality=96&type=album)
Перезагрузил файл для сохранения настроек с помощью команды sudo pg_ctlcluster 12 main reload и просмотрел содержимое файла:
![avatar](https://sun9-west.userapi.com/sun9-2/s/v1/ig2/uBq_liNiDMMjlHX3ia5A0PdSGP5Z2w0xu63KHrfYGeroQ6cYyuiqSDotWlI3OtDVXyW07w1p3kwMIuJeONH7wviU.jpg?size=590x225&quality=96&type=album)
Проверил подключение. Подключился как пользователь kat к тестовой БД bd1:
![avatar](https://sun9-87.userapi.com/impg/qawpIlDhDBnnmI54_-NW6SS7gIBiPwn0AcDSvg/hxeZkMYj5Kg.jpg?size=805x69&quality=96&sign=d37360eefe412a35b9ae69c3a497e24a&type=album)
На снимке видно, что подключение прошло успешно.

