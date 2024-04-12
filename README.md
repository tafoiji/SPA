# SPA
## Задание 1. 
Создать новый проект, в который добавить одну страницу - index.html. Это страница Single Page Application (SPA), которая может отображать два вида страниц:
- на главной странице приложения должна быть размещена общая информация о приложении и кнопка перехода на вторую страницу;
-	на второй странице должна отображаться информация по предметной области согласно варианта. 

## Задание 2. 
2.1 Создать json файл, в котором хранятся данные согласно предметной области. Структура данных аналогична той, что использовалась в лаб.3-4. Например, для варианта «Ботанический сад» ключ – название растения, значение – описание ухода за растением, для варианта «Периодические издания» ключ – название издания, значение – описание издания (или стоимость – по желанию). Аналогично для остальных вариантов.
Информация для второй страницы SPA - приложения должна подгружаться из этого JSON­файла через AJAX и отображаться в виде таблицы.

2.2 Развернуть  SPA приложение на сервере Express (https://expressjs.com/ru/). Для этого создать новый JS проект, в который добавить зависимость: express. 
Перенести в этот проект страницу index.html задания 1.
Для запуска сервера express создать конфигурационный файл сервера – server.js. В настройках маршрутизации этого файла предусмотреть два url: по запросу к первому url отдается страница index.html (response.sendFile()), по запросу ко второму url происходит скачивание файла (response.download ()) из п.2.1.
