# ghuserinf
Задание
Написать приложение для отображения информации о пользователе GitHub и списка его репозиториев в соответствии с дизайном.

Дизайн

<img src="https://startup-summer-task.paralect.com/_next/image?url=https%3A%2F%2Fapi.super.so%2Fasset%2Fstartup-summer-task.paralect.com%2Fbf6d96fa-29ff-48aa-af17-b46f78d86945.png&w=750&q=100">

Требования

Используй create-react-app для создания приложения .
Храни код своего приложения в GitHub. 
[Инструкция](https://docs.github.com/en/github/getting-started-with-github/create-a-repo)
Чтобы твоё приложение было доступно по ссылке, как и любой другой сайт, его нужно задеплоить. Используй Vercel. 
[Инструкция](https://vercel.com/guides/deploying-react-with-vercel-cra)


Функциональность

На странице должна быть поисковая строка для ввода username пользователя.
При вводе username и нажатии кнопки Enter происходят запросы на API GitHub. При получении ответов от сервера необходимо отобразить данные пользователя и список его репозиториев.
💡
Для выполнения тестового задания тебе понадобятся эти эндпоинты GitHub:
- [List repositories for a user](https://docs.github.com/en/rest/reference/repos#list-repositories-for-a-user)
- [Get a user](https://docs.github.com/en/rest/reference/users#get-a-user)


При нажатии на username пользователя, должен открыться его профиль в новой вкладке.
💡
Используйте поле html_url из полученного профиля пользователя в качестве ссылки.

При нажатии на имя репозитория, должна открыться его страница в новой вкладке.
💡
Используйте поле html_url из полученного списка репозиториев в качестве ссылки.

Дополнительная функциональность
Отображать loader - [(пример)](https://www.w3schools.com/howto/howto_css_loader.asp) во время ожидания ответа сервера
Показывать отдельную страницу (empty state), если у пользователя нет репозиториев
Показывать отдельную страницу (empty state), если пользователя с username не существует.
Реализовать постраничный просмотр репозиториев. Можно использовать [react-paginate](https://www.npmjs.com/package/react-paginate)
Минимальная ширина страницы, при которой она отображается корректно – 320 рх. Все указанные в задании элементы присутствуют как на десктопной, так и на мобильной версии
