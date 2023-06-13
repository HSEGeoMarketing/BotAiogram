В этом репозитории представлен Telegram-бот, реализованный с использованием aiogram. Бот обладает различными функциональностями, включая анализ данных для розничных магазинов и оценку посещаемости на основе адреса и площади.
Данный бот предоставляет удобный интерфейс для взаимодействия с различными функциями. Вы можете использовать команды бота для получения информации о розничных магазинах, анализа данных и оценки посещаемости.

## Команды бота
Бот поддерживает следующие команды:

- `/start` - Запустить бота и начать диалог.
- `/help` - Показать справку по доступным командам.
- `/quit` - Завершить работу бота
- `Топ-5 мест для магазина`(команда 1) - Вывод списка топ-5 магазинов для розничной сети с указанием адреса, посещаемости, стоимости и других параметров.
- `Проходимость по адресу`(команда 2) - Оценка предполагаемой посещаемости на основе адреса и площади магазина.

Вы можете использовать эти команды, чтобы взаимодействовать с функциональностями бота.

## Обработка данных
Бот позволяет выполнять несколько запросов одновременно, используя aiogram и asyncio.
При использовании команды 1, бот запросит название розничной сети и выдаст 5 лучших мест, найденных на сайте Авито, с их характеристиками, а также информацию о посещаемости и стоимости одного посетителя. Кроме того, бот предоставит карту для каждого места из топа, на которой будут указаны конкуренты и жилые дома в радиусе 400 метров.
При использовании команды 2, бот запросит адрес и площадь помещения, а затем предоставит оценку предполагаемой посещаемости. Бот также предоставит карту для указанного места, на которой будут отображены конкуренты и жилые дома в радиусе 400 метров.
Для выполнения функций анализа данных и оценки посещаемости, бот использует модели машинного обучения, разработанные с использованием библиотек CatBoost и PyTorch.

## Результаты работы команд
Каждая команда предоставляет соответствующую информацию или результаты пользователю.
Различные команды бота возвращают разные результаты. Ниже приведены примеры результатов работы команд:
