# naumenTestTask
naumenTestTask
Приложение, с помощью которого можно искать текстовую
информацию в Wikipediа, испольующее открытое API Wikipedia.
-
1. Интерфейс
Пользователь вводит свой запрос в предназначенную для этого форму поиска, нажимает кнопку "Найти" и получает список статьей 
по своему запросу из  википедии с заголовоком статьи, с ссылкой на нее и краткуой информацией о статье (сниппет).
2. Передача данных, логика работы приложения
После ввода запроса и нажатия кнопки "Найти" или Enter из введённого в форму поиска запроса пользователя, 
формируется GET запрос к API Wikipedia и выводится список статьей из википедии.
3. Структура, описание реализации приложения
При нажатии кнопки "Найти" или Enter запускается функция в которой вначале в переменную записывается ссылка для формирования
GET запроса и если введённый запрос пользователя не пустой, то с использованием AJAX если GET запрос прошёл успешно, то 
обновляем поле вывода и записываем туда все полученные при помощи GET запроса заголовоки статьи, с ссылкой 
на них и краткой информацией о статье (сниппет). Если GET запрос не прошёл успешно, то выводим оповщение об ошибке - "error".
Далее реализована функция для запуска поиска не только с кнопки, но и при нажатии на кнопку Enter.
-
Попробовать приложение можно здесь - http://htmlpreview.github.com/https://github.com/grishbar/naumenTestTask/blob/master/index.html
