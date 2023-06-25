# Перечень автоматизируемых сценариев
### Способы перехода на страницу курса Тестировщик ПО с главной страницы сайта Нетология:
1. кнопка “Каталог курсов” → в направлениях обучения кнопка “Все курсы”→ в строке “Какой курс Вам нужен?” набрать “Тестировщик” → кнопка “Найти курс”→ выбрать в списке курс “Тестировщик ПО”
2. кнопка “Каталог курсов” → в направлениях обучения кнопка “Все курсы”→ в строке “Какой курс Вам нужен?” набрать “Тестировщик” → в высветившихся вариантах выбрать “Тестировщик ПО”
3. кнопка “Каталог курсов” → кнопка “Программирование”→выбрать в списке курс “Тестировщик ПО”
4. кнопка “Каталог курсов” → в строке “Какой курс Вам нужен?” набрать “Тестировщик” → в высветившихся вариантах выбрать “Тестировщик ПО”
5. в “Направления обучения” выбрать “Программирование” → выбрать в списке курс “Тестировщик ПО”
6. в “Направления обучения” выбрать “Полный каталог” → в строке “Какой курс Вам нужен?” набрать “Тестировщик” → кнопка “Найти курс”→ выбрать в списке курс “Тестировщик ПО”
7. внизу главной страницы в столбце “Обучение” кнопка “Каталог курсов” → в строке “Какой курс Вам нужен?” набрать “Тестировщик” → кнопка “Найти курс” → выбрать в списке курс “Тестировщик ПО”
8. внизу главной страницы в столбце “Обучение” кнопка “Программирование” → выбрать в списке курс “Тестировщик ПО”
9. внизу главной страницы в столбце “Обучение” кнопка “Популярные курсы” → выбрать в списке курс “Тестировщик ПО”
## Способы перехода к заполнению формы:
1. пролистать всю страницу профессии до формы записи
2. нажать кнопку “Записаться” на первоначально высветившемся экране возле кнопки “Посмотреть программу”
3. пролистать страницу ниже и нажать на кнопку “Записаться”, появившуюся в верхнем правом углу
## Сценарии заполнениях формы записи:
| № |Предусловие     | Шаги                                       | Пример                                       | Ожидаемый результат                                          | 
|---|----------------|--------------------------------------------|----------------------------------------------|--------------------------------------------------------------|
| 1 | Пользователь не авторизован | 1. Ввести действительное имя на русском языке;   2. Ввести действующий телефон, гигиена с 8; 3. Нажать «Записаться». | Александр 8(952)85-96-76-386                 | Заявка отправлена                                                                                                                                            |
| 2 | Пользователь не авторизован | 1. Ввести имя на русском языке с буквой Ё; 2. Ввести действующий телефон, гигиена с +7; 3. Нажать «Записаться».     | Ёко +7(952)85-96-76-386                      | Заявка отправлена                                                                                                                                            |
| 3 | Пользователь не авторизован | 1. Ввести действительное имя на русском языке с дефисом;  2. Ввести действующий телефон; 3. Нажать «Записаться».    | Мария-Владислава 8(952)85-96-76-386          | Заявка отправлена                                                                                                                                            |
| 4 | Пользователь не авторизован | 1. Ввести действительное имя на русском языке из 1 буквы;  2. Ввести действующий телефон; 3. Нажать «Записаться».   | О 8(952)85-96-76-386                         | Заявка отправлена                                                                                                                                            |
| 5 | Пользователь не авторизован | 1. Ввести действительное имя на русском языке из 25 букв;  2. Ввести действующий телефон; 3. Нажать «Записаться».   | Ааааааааааааааааааааааааа 8(952)85-96-76-386 | Заявка отправлена                                                                                                                                            |
| 6 | Пользователь не авторизован | 1. Ввести имя на русском языке из 26 букв;  2. Ввести телефон из 10 цифр; 3. Нажать «Записаться».                   | Аааааааааааааааааааааааааа 8(952)85-96-76-38 | Заявка не отправлена. Под полем имя написано “Должно быть не более 25 символов” Под полем телефон написано “Номер в формате +9 (999) 999-99-99”              |
| 7 | Пользователь не авторизован | 1. Ввести цифры в поле имени; 2. Ввести телефон из 12 цифр; 3. Нажать «Записаться».                                 | 123 8(952)85-96-76-3863                      | Заявка не отправлена. Под полем имя написано “Может содержать только русские буквы и дефис”. Под полем телефон написано “Номер в формате +9 (999) 999-99-99” |
| 8 | Пользователь не авторизован | 1. Ввести имя на иностранном языке; 2. Ввести телефон из 1 цифры; 3. Нажать «Записаться».                           | Petr 8                                       | Заявка не отправлена. Под полем имя написано “Может содержать только русские буквы и дефис”. Под полем телефон написано “Номер в формате +9 (999) 999-99-99” |
| 9 | Пользователь не авторизован | 1. Ввести в поле имя спецсимволы; 2. Оставить поле телефона пустым; 3. Нажать «Записаться».                         | —--                                          | Заявка не отправлена. Под полем имя написано “Может содержать только русские буквы и дефис”. Под полем телефон написано “Поле обязательно для заполнения”    |
| 10| Пользователь не авторизован | 1. Ввести имя на русском языке с пробелом; 2. Ввести действующий телефон; 3. Нажать «Записаться».                   | Пе тр 8(952)85-96-76-386                     | Заявка не отправлена. Под полем имя написано “Может содержать только русские буквы и дефис”.                                                                 |
| 11| Пользователь не авторизован | 1. Оставить поле имя пустым;  2. Ввести действующий телефон; 3. Нажать «Записаться».                                |  8(952)85-96-76-386                          | Заявка не отправлена. Под полем имя написано “Поле обязательно для заполнения”.                                                                              |
| 12| Пользователь авторизован    | 1. Нажать “Записаться”                                                                                              |                                              | Заявка отправлена                                                                                                                                            |

# Перечень используемых инструментов:
* *IntelliJ IDEA* : отличается обширным набором инструментов для рефакторинга (перепроектирования) и оптимизации кода.  Доступна функция Run Targets, позволяющая запускать, тестировать и отлаживать приложения в Docker-контейнерах, на удаленных SSH-серверах и в WSL. Доступны инструменты для проведения автоматических тестов и формирования аналитики, которая показывает, какой объем кода протестирован, отладчик, показывающий значения переменных прямо в исходном коде, возможность выбрать метод отладки, встроенный декомпилятор — инструмент для преобразования исполняемого двоичного кода из jar-файлов в читаемый Java-код.
* *Java* : удобное написание тестов в IntelliJ IDEA. Много инструментов для автотестированиямножество фреймворков и библиотек, покрывающих самые популярные протоколы и сервисы.
* *Junit 5* : фреймворк для Java, полностью совместимый с самим языком и его инструментами. Гибкие настройки. Позволяет параллельно запускать несколько тестов или объединять разные тестовые программы в набор. Есть встроенное правило, которое позволяет задать тайм-аут. Возможность создавать и запускать динамические тесты.
* *Lombok* : библиотека для сокращения кода в классах и расширения функциональности языка Java. Избавляет от ручного набора однотипных фрагментов кода и предотвращает появление ошибок. Экономит время. Улучшает читаемость кода.
* *Selenide* предлагает лаконичный API для использования Selenium WebDriver в UI тестах: умные ожидания, автоматическое управление браузером, предлагает лаконичный и мощный API, автоматические скриншоты, удобные методы для заполнения полей, выбора чекбоксов, выпадающих списков, поиска элементов по тексту и т.д.
* *Gradle* : удобная и гибкая настройка, более производительный запуск тестов.
* *Git* и *GitHub* : получение информации о репозитории, сравнение файлов, переключение между различными ветками, откат изменений, настраивание удобной и информативной консоли, решение конфликтов кода, кроссплатформенность, эффективные code-review, реализование CI / CD.
* *Appveyor* : непрерывная интеграция, которая создает и тестирует код каждый раз, когда он отправляется в репозиторий Git, гарантируя, что ошибки будут быстро обнаружены. Может быть интегрирован с проектами GitHub и поддерживает частные проекты.
* *Allure* : построение понятной и прозрачной автоматизации с нуля: от написания теста до аналитики по результатам десятков прогонов.

# Перечень необходимых разрешений, данных и доступов
* Разрешение на тестирование и автоматизацию сайта ООО “Нетология”
* Тестовые данные для заполнения формы либо доступ к базе данных
* Доступ к авторизированному аккаунту

# Перечень необходимых специалистов для автоматизации
Необходим 1 тестировщик-автоматизатор с умением пользоваться указанными выше инструментами.

# Интервальная оценка с учётом рисков в часах
Интервальная оценка тестирования составляет 48 часа рабочего времени.

# Перечень и описание возможных рисков при автоматизации
* Учитывая, что объем работы не является большим, настройка проекта и его автоматизации могут повлечь бОльшие временные и финансовые затраты в сравнении с ручным тестированием
* Задействование многих других страниц сайта при переходе к странице курса “Тестировщик ПО” может повлечь быстрое устаревание тестов
* Отсутствие у большинства элементов явных селекторов может привести к увеличению сроков выполнения работы, ошибкам и, при наличии изменений в будущем, появлению недействительного кода