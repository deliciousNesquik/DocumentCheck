# DocumentCheck (Проверка документов)


## Определение проблемы:
Проект который должен упростить проверку документов на валидность
данных в такой сфере как Бухгалтерия. Проблема состоит в том что
при загрузке документа в общую систему документов, 
система при нахождении ошибки завершает проверку до момента исправления
при этом каждая ошибка тормозит процесс загрузки документа в систему.


## Выработка требований:
Программа должна уметь автоматизированно проверять документы которые в нее загружает пользователь
на валидность

1) Умение регистрировать пользователя в системе.
2) Возможные подсказки пользователю для более легкой работы в программе.
3) Создание пользовательской проверки документов.
4) Возможность делиться пользовательскими проверками документов.
5) Возможность редактирования, удаления пользовательской проверки документов.
6) Автоматизированная проверка документов.
   

## Разработка архитектуры:

### Общее описание системы:


### Основные компоненты:
Windows Presentation Foundation - система для построения клиентских приложений Windows. Основной компонент системы.

Excel Document Check - компонент, получающий файл excel от пользователя и обрабатыаающий его для дальнейшего исправления или других  иных действий. Основной компонент системы.

Компонент создания пользовательский проверки документов - компонент, необходимый для лёгкого создания, редактирования и удаления пользовательский проверки документов в системе, а так же для того чтобы делиться данными проверками с другими пользователями.

Служба обновления - компонент, который служит для поиска и обновление системы до новейшей версии для поддержания стабильности работы системы.

Служба авторизации пользователя - компонент, служащий для регистрации пользователя в системе.

Служба журналирования действий системы, служба для хранения истории действий пользователя и программы для корректного нахождения ошибок и сбоев системы 


### Формат и способ хранения данных:
Файлы логирования будут иметь структуру 
(дата время)_(имя системы).txt 

Файлы для хранения пользовательских настроек будут называться
config_(имя пользователя).ini

Файлы для хранения пользовательских проверок документов будут иметь структуру названия 
(имя пользователськой проверки).check

### Способ организации пользовательского интерфейса:


### Подход к безопасности системы:


### Оценки производительности:


### Возможности масштабирования:


### Моменты, связанные с интернациональностью, т.е. будет ли система интернациональной:





