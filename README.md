# Телефонный справочник

1. Контроллер
    * управляет всей программой
2. Интерфейс
    * Сложнота так как выборов очень много - По сути - интерфейс это набор функций приветсвий, выборов , текста и вывода 
3. Модуль Ввода
    * Нужно определиться со Столбцами справочника + если есть что-то повторяющееся, к примеру пол - вывести отдельный словарь.
4. Модуль Вывода
    * Стоит выбрать 1 язык, будет время - добавить другие
5. Логирование

Структура базы

|Поля Справочника | Type | Comment |
| ----- | ----- | ----- |
|Фамилия | str| |
|Имя | str | |
|пол | str | |
|тип| str ||
|телефон| str|

1. старт программы [main](main.py)
2. контроллер [controller](controller.py)
3. Интерфейс [interface](interface.py) [scheme](interface_scheme.drawio)
4. Ввод информации [input](input_name.py)
    * нужно доделать
5. Вывод информации [output](data_output.py)
6. База данных [Data_Base](phone_numbers.json)
    * Пока что есть 1 база
    * В изначальном плане было 3 бызы
        1. Кталог, куда информация только заносится и не удаляется
        2. Актуальная база - где хранятся только те контакты которые не удалялись с 1.
        3. База удалённых позиций ( ну что бы было)
    * Изначальный вариант предполагал , что у человека будет несколько номеров
        1. Долго играющий проект, поняли что никак не успеем
        2. Модуль создания базы и вывода карточек в принцепе готов
        3. Сложность Словарь в Словаре в Словаре =)
7. Словари для использования [dicts](dict/dictionarys.py)
8. Создание ряда, внос и вынос из базы [base_use](worck_with_base)
9. Поиск/Замена/Удаление записи [wotck_wit_card](Look_up_delete_add)

Планы на будущее:  
    - [ ] Доделать Модуль ввода и проверок  
    - [ ] Вывести из контроллера всё в функции  
    - [ ] Дооформить контроллера  
    - [ ] Добавить Loger   
    - [ ] Добавить Импорт и Экспорт в другие форматы  
    - [ ] Улучшить базу для нескольких номеров у одного человека  
