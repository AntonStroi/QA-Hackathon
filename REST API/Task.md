# Написання тест кейсів на ендпоінт (REST API) по Swagger документації
***Завдання:*** Надати учасникам доступ до Swagger-документації для API сервісу, що обробляє запити від мобільного застосунку. Мета — розробити тестові кейси для основних REST API ендпоінтів, включаючи позитивні та негативні сценарії.

***Ключові кроки:***
- Аналіз Swagger документації для розуміння методів API (GET, POST, PUT, DELETE).
- Написання тест кейсів для кожного з методів, враховуючи різні статуси відповідей (200 OK, 404 Not Found, 500 Internal Server Error).
- Симуляція некоректних запитів (наприклад, з неправильною авторизацією або відсутніми полями).
- Створити невелику Postman колекцію, з ланцюжком 3-4 запита, логічно пов’язаних один з одним, використовуючи Swagger документацію.
- Рішення залити на github у вигляді експортованої колекції.

***Інструменти:***
Тобі знадобиться: Postman, GitHub акаунт

---

***Завдання 1.***

Створить невелику Postman колекцію, з ланцюжком 3-4 запита, логічно пов’язаних один з одним, використовуючи Swagger документацію за посиланням [Swagger UI](https://petstore.swagger.io/). Також проаналізуйте документацію на неспівпадіння статус кодів або запропонуйте покращення. Рішення надати у вигляді експортованої колекції.

***Requirements:***

- У запитах не повинно бути (або мінімум) статичних даних. Необхідно використовувати на вибір: вбудовані функції postman для генерації даних або Pre-Request Script
- Колекцію можна запустити всю повністю за допомогою рана в postman без редагування.
- До кожного запиту мають бути тести. Розробка тестів та їх кількість (мінімум 1 тест) повністю на розсуд учасника.

Приклад: створити сутність, отримати сутність, відредагувати сутність, отримати сутність повторно.

***Завдання 2.***

До будь якого ендпоінта, обраного у попередньому завданні, написати до 10 тесткейсів, які покривають ендпоінт.

Рішення завдання 1 і завдання 2 залити на github у папку ***REST API***. Воно повинно включати всі необхідні файли для запуску колекції (завдання 1), аналіз документації у файлі Analyse (завдання 1) і README (завдання 2). Надати лінку на github з рішенням.

---

# Help guide
1. У запитах не повинно бути (або мінімум) статичних даних. Необхідно використовувати на вибір: вбудовані функції postman для генерації даних або Pre-Request Script

- [Write pre-request scripts to add dynamic behavior in Postman | Postman Learning Center](https://learning.postman.com/docs/tests-and-scripts/write-scripts/pre-request-scripts/)
- [Reuse data with variables and environments in Postman | Postman Learning Center](https://learning.postman.com/docs/sending-requests/variables/variables-intro/)
- [Use dynamic variables to return randomly generated data | Postman Learning Center](https://learning.postman.com/docs/tests-and-scripts/write-scripts/variables-list/)

***Pre-Request Script example:***

`"var pet_id = pm.variables.replaceIn('{{$randomInt}}')"`
`"pm.environment.set("PET_ID", parseInt(pet_id));"`

2. До кожного запиту мають бути тести. Розробка тестів та їх кількість (мінімум 1 тест) повністю на розсуд учасника.

- [Postman test script examples | Postman Learning Center](https://learning.postman.com/docs/tests-and-scripts/write-scripts/test-examples/)

3. Колекцію можна запустити всю повністю за допомогою Run collection в Postman без редагування.

- [Test your API using the Collection Runner | Postman Learning Center](https://learning.postman.com/docs/collections/running-collections/intro-to-collection-runs/)

Приклад: створити сутність, отримати сутність, відредагувати сутність, отримати сутність повторно.

5. За посиланням ви знайдете [Приклад колекції з одного запиту](https://github.com/AntonStroi/QA-Hackathon/blob/main/REST%20API/postman_collection.json)

6. За посиланням ви знайдете [Приклад оформлення тест кейсів](https://github.com/AntonStroi/QA-Hackathon/blob/main/REST%20API/README.md)

7. Як створити репозиторій і залити туди рішення: [GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

---

# Успіхів!

---