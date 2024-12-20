# Аналіз вимог і написання тест кейсів до задачі 
***Завдання:*** Учасники мають проаналізувати мобільний додаток і виходячи з результатів сформувати список тест кейсів, який би включав перевірки існуючого функціонала з інтеграцією нової фічі. 

***Ключові кроки:**()

- Exploratory testing.
- Аналіз вимог задачі.
- Написання тест кейсів.

***Інструменти:***

- Мобільні емулятори (Android Studio).

---
# Завдання

1. Провести exploratory testing функціоналу, який може стосуватися вимог задачі.
2. Проаналізувати вимоги до задачі і написати тест кейс або тест кейси до задачі описаної нижче. 

***Задача:***

- При переході по картці Do Your Workout з Personal plan екрану користувач потрапляє в Trainings Tab - [Design](https://lh7-eu.googleusercontent.com/docsz/AD_4nXe-T7f6gCax5eu2asB-qv64NFlbs_mh6Vd5Uur62QIliJkCihp-9lYm0fz8I2BoD4hr3F-j8l0Lon38Ep_9C17ijZHyH1tpeCO7hC9tjeIrQHjLOC78CV2C4T_abzb_MspPIWrUSP5XngtxYaXI2YsKpHA?key=_6zRhVjU3ecnt-VpyHY-Eg).

- В табі Trainings новий блок: Today’s Activity, в якому знаходяться від 1 до 3 рекомендованих тренувань, в залежності від кількості обраних користувачем activity на онбордінгу [Design](https://lh7-eu.googleusercontent.com/docsz/AD_4nXcUv44DluYy7Axok2VU31lCHrM4Y7AzVnJOkVe-49ERsHuJTYB40Z3xMR8LPcJ6Cx8KhJYWqYEChVXYhegeQmhjhspz9_N5vd0Ec3t80skujLdeT5PO2ifo7KqkJ96kBfAzGOHVpoYiJBtc4tdez8TKxuM?key=_6zRhVjU3ecnt-VpyHY-Eg).

- Title - “Recommended for you”. Subtitle - “Get daily workouts tailored to your goal and interests in [Chosen Activity #1], [#2] and [#3].”

- Якщо активності обрані тільки 2, пишемо 2, якщо тільки одна то відповідно пишемо interest (без множини): “Get daily workouts tailored to your goal and interest in [Chosen Activity #1].”
[Design](blob:https://newsiteam.atlassian.net/879312bd-49d7-43cc-be95-b7d13cb2293f#media-blob-url=true&id=6434d88c-26f7-42ae-805d-a74245035684&collection=contentId-4601839635&contextId=4601839635&mimeType=image%2Fpng&name=image-20240214-072503%20(1).png&size=19139&width=286&height=68&alt=image-20240214-072503%20(1).png)

- Якщо користувач обрав 2 і більше рекомендованих activity
   - При виконані 1 з них ми замінюємо Subtitle: “Great job! [N] more workout left” - [Design](blob:https://newsiteam.atlassian.net/9864e57b-9808-4284-8230-710f177181cd#media-blob-url=true&id=97b9bf09-8aff-496e-b8d5-628f4eb4ed7d&collection=contentId-4601839635&contextId=4601839635&mimeType=image%2Fpng&name=image-20240214-073702%20(2).png&size=151738&width=367&height=280&alt=image-20240214-073702%20(2).png).
   - При виконані всіх ми замінюємо Subtitle: “All workouts done! For an extra challenge, check out the workout library below” - [Design](blob:https://newsiteam.atlassian.net/d24556ba-86a9-42d2-99a8-3ed18c969ea3#media-blob-url=true&id=c3d43049-622d-4b5e-affb-833a3a4c7fb3&collection=contentId-4601839635&contextId=4601839635&mimeType=image%2Fpng&name=image-20240214-073821%20(1).png&size=165965&width=361&height=315&alt=image-20240214-073821%20(1).png).
   - На екрані Personal plan відмічаємо картку Do Your Workout як виконану.
- Вся область карточки клікабельна та переводить на Workout preview screen

- ***Нотатка до завдання:*** Екран з вибором activity користувач бачить під час проходження онбордінгу як гість або після реєстрації - [Design](blob:https://newsiteam.atlassian.net/fd7ca4af-91e4-4c4b-9849-635645917e05#media-blob-url=true&id=b1a3fd34-e278-4046-afaa-858a893a6db2&collection=contentId-4601839635&contextId=4601839635&mimeType=image%2Fjpeg&name=photo_2024-06-25%2019.18.15%20(1).jpeg&size=59764&width=606&height=1280&alt=photo_2024-06-25%2019.18.15%20(1).jpeg)

Рішення залити на github у папку ***Requirements analysis.*** В README написати тест кейси або тест кейси до задачі.

---

# Help guide
- Додаток можна завантажити за посиланням [Better Me](https://play.google.com/store/apps/details?id=com.gen.workoutme&hl=en)

- Як створити репозиторій і залити туди рішення: [GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

---

# Успіхів!

---