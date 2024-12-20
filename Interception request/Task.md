# Проксування запитів за допомогою debug proxy інструментів (Charles/Fiddler)
***Завдання:*** За допомогою інструментів проксування (наприклад, Charles Proxy або Fiddler) учасники мають перехопити HTTP/HTTPS-запити і перевірити, які саме дані передаються між клієнтом і сервером.

***Ключові кроки:***

- Налаштування проксі для перехоплення запитів від застосунку.
- Аналіз запитів на відповідність специфікаціям API та коректність даних.
- Виявлення помилок або зайвих запитів, які можуть вплинути на продуктивність.

***Інструменти:***

Тобі знадобиться: Postman, Charles Proxy, Fiddler або Proxyman

---

# Завдання

1. Перейти на веб сторінку https://demo.owasp-juice.shop/#/login в мобільному браузері на емуляторі або реальному девайсі.
2. Зареєструватися. 
3. Перевірити реакцію додатку на повернення різних статус кодів на ендпоінт POST/rest/user/login. 

- 400 - Happens when no json body passed or json is malformed
- 401 - Unauthorized
- 409 - This purchase already exists
- 422 - Happens when there're some troubles with data, submitted by client (validation errors, playstore validation errors)
- 429 - Happens when we exceeded google api limits
- 500 - Something bad happend on a server
- 502 - Application temporary down because of laggy network connection or restart process

Рішення залити на github у папку ***Interception request.*** Воно повинно включати всі необхідні  відео файли (не довші 1 хвилин, назва відео співпадає з кодом помилки - 400, 401 тощо). Додати README файл з заведеним одним багом (оформлення на власний розсуд з дотриманням best practice).

---

# Help guide
- Налаштуйте debug proxy інструмент
Скачать з оф. сайта - [Download a Free Trial of Charles • Charles Web Debugging Proxy](https://www.charlesproxy.com/download/)

***Як налаштувати Charles:***

1. Після установки треба підключити девайс до комп'ютера. 
2. Відкрийте налаштування wifi на девайсі
3. Натисніть властивості (advanced)
4. У HTTP PROXY розділі оберіть Manual
5. Введіть ip адресу вашого комп'ютера (через терминал Win - ipconfig)
6. Введіть proxy порт (8888 - за замовчуванням)
7. Дозвольте підключеному пристрою переглядати трафік через ваш проксі (на вашому комп'ютері).
8. Також необхідно встановити сертифікати на пристрої для розшифрування різних запитів HTTPS-трафіку:
 - Налаштуйте пристрій для використання Charles як його HTTP-проксі на <IP-адрес вашої робочої станції>
 - На девайсі відкрити http://chls.pro/ssl 
 - Установити Certificate

***Корисні відео***
За посиланням [Interception request](https://github.com/AntonStroi/QA-Hackathon/tree/main/Interception%20request) ви знайдете:
1. Відео як підключити проксі на емуляторі (Charles): 1-setup-charles-for-proxying-test-app
2. Приклад як відео з перехопленням і підміною респонс кода: 2-enable-proxy-and-intercepting-a-login-request
3. Документація як використовувати інструменти:
- [Breakpoints Tool • Charles Web Debugging Proxy](https://www.charlesproxy.com/documentation/proxying/breakpoints/)
- [Rewrite Tool • Charles Web Debugging Proxy](https://www.charlesproxy.com/documentation/tools/rewrite/)
4. Як створити репозиторій і залити туди рішення: [GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

---

# Успіхів!

---