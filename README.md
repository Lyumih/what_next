# what_next
Когда в построении сайта ты не знаешь, что делать дальше, воспользуйся данным виртуальным помощником.


# Пример: Создание сайта с нуля
1. Вы хотите создать новый сайт, приложение, книгу?
- сайт (выбрать, изучено)
- приложение  (выбрать, не изучено)
- книга (выбрать, не изучено)
(Выбрано: 1)
2. Давайте создадим минимальную начальную страницу.
- Создайте файл index.html (готово, не изучено)
- Дайте название файлу "Мой сайт" в теге <title></title> (в процессе, изучено)
- Напечатать фразу "Содержание сайта" в теге <body></body> (в ожидании, изучено)

3. И т.д.

# Ключевые моменты помощника
1. Помощник статрается предугадать ход ваших мыслей и преложить несколько вариантов.
2. К каждому варианту прилагается справочный материал, который поможет освоить данный шаг.
3. Можно взаимодействовать с помощником.
4. Помощник включает в себя лучшие практики программирования.
5. Вы можете добавлять свои варианты действий для помощника.

# Пример: добавить своё действие для помощника.
1. Вы хотите добавить действие для помощника? (выбрать, изучено)
- Вы хотите редактировать действие для помощника? (выбрать, не изучено)
- Вы хотите удалить действие для помощника? (выбрать, не изучено)
(Выбрано: 1)

2. Расскажить об данном действии
- Дать имя
- Рассказать алгоритм выполнения
- Добавить справочный материал
- Как понять, что действие выполнено?

# Структура помощника
Лучше всего представить структуру помощника в виде меню-аккордиона.
Где заголовки меню - это название шагов помощника.
А раскрывающиеся подменю - это название действией для выполнения шагов.

Шаг 1 (procee, info)
- Действие 1 (do, info)
- Действте 2 (done, info)
- Действие 3 (process, info)

Шаг 2 (done, info)

Шаг 3 (do, info)

# JSON для помощника
Открыть на сайте https://jsoneditoronline.org/?id=baa1b887f7d346d09185bca662b9a378  
И вставить json текст ниже  

{
  "helper": {
    "name": "Мяу-кот создатель сайтов",
    "discripton": "Кот помогает создать сайты новичкам",
    "steps": [
      {
        "name": "Чем я могу вам помочь?",
        "status": "process",
        "info": {
          "link": "www.lernjs.ru",
          "description": "ссылка на описание 1 шага помощника",
          "status": "lern"
        },
        "actions": [
          {
            "name": "Создать новый проект",
            "status": "do",
            "info": {
              "link": "www.lernjs.ru",
              "description": "ссылка на описание 1 шага 1 действия помощника",
              "learn": true
            }
          },
          {
            "name": "Открыть существующий проект",
            "status": "process",
            "info": {
              "link": "www.lernjs.ru",
              "description": "ссылка на описание 1 шага 2 действия помощника",
              "learn": false
            }
          }
        ]
      }
    ]
  }
}
