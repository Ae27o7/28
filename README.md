# 28
final test
Финальное задание курса "Тестировщик-автоматизатор на Python
В качестве объекта теcтирования выбран сайт https://www.labirint.ru/

tests/ содержит тесты для главной старницы (отдельно для header, body, footer), страницы поиска, корзины и страницы товара. pages/base.py содержит реализацию шаблона PageObject для Python
pages/elements.py содержит вспомогательный класс для определения веб-элементов на веб-страницах

Как запускать тесты:
Установить все внешние зависимости командой
pip install -r requirements.txt

Скачать версию Selenium WebDriver, совместимую с вашим браузером
(тесты проводились в браузере Google Chrome)

Запуск тестов командами:

python -m pytest -v --driver Chrome --driver-path ${PATH_TO_DRIVER} tests/test_main_page_header.py

python -m pytest -v --driver Chrome --driver-path ${PATH_TO_DRIVER} tests/test_main_page_body.py

python -m pytest -v --driver Chrome --driver-path ${PATH_TO_DRIVER} tests/test_main_page_footer.py

python -m pytest -v --driver Chrome --driver-path ${PATH_TO_DRIVER} tests/test_search.py

python -m pytest -v --driver Chrome --driver-path ${PATH_TO_DRIVER} tests/test_book_page.py

python -m pytest -v --driver Chrome --driver-path ${PATH_TO_DRIVER} tests/test_card_page.py

где ${PATH_TO_DRIVER} находится путь к драйверу Selenium для текущей ОС
