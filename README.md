# Vkgrouptester
Задание
Задание: Вывести список групп в ВК в которых состоит пользователь, но не
состоит никто из его друзей. В качестве жертвы, на ком тестировать, можно
использовать: https://vk.com/tim_leary

ВХОДНЫЕ ДАННЫЕ:
Имя пользователя или его id в ВК, для которого мы проводим
исследование
Внимание: и имя пользователя (tim_leary) и id (5030613) - являются
валидными входными данными
Ввод можно организовать любым способом:
• из консоли
• из параметров командной строки при запуске
• из переменной

ВЫХОДНЫЕ ДАННЫЕ:
файл groups.json в формате
[
{
“name”: “Название группы”,
“gid”: “идентификатор группы”,
“members_count”: количество_участников_собщества
},
{
…
}
]
Форматирование не важно, важно чтобы файл был в формате json

ТРЕБОВАНИЯ К ПРОГРАММЕ:
• Программа не падает, если один из друзей пользователя помечен как “удалён” или
“заблокирован”
• Показывает что не зависла: рисует точку или чёрточку на каждое обращение к api
• Не падает, если было слишком много обращений к API
(Too many requests per second)
Ограничение от ВК: не более 3х обращений к API в секунду.
Могут помочь модуль time (time.sleep) и конструкция (try/except)
• Код программы удовлетворяет PEP8

КАК ИСПОЛЬЗОВАТЬ ПРОГРАММУ: 

Запустите скрипт
Передайте ему имя пользователя или id
Получите список групп