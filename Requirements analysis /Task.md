# Аналіз вимог і написання тест кейсів до задачі 
***Завдання:*** Учасники мають проаналізувати мобільний додаток і виходячи з результатів сформувати список тест кейсів, який би включав перевірки існуючого функціонала з інтеграцією нової фічі. 

***Ключові кроки:***

- Exploratory testing.
- Аналіз вимог задачі.
- Написання тест кейсів.

***Інструменти:***

- Мобільні емулятори (Android Studio), GitHub акаунт.

---
# Завдання

- Додаток можна завантажити за посиланням [Better Me](https://play.google.com/store/apps/details?id=com.gen.workoutme&hl=en)

1. Провести exploratory testing функціоналу, який може стосуватися вимог задачі.
2. Проаналізувати вимоги до задачі і написати тест кейс або тест кейси до задачі описаної нижче. 

***Задача:***

- При переході по картці Do Your Workout з Personal plan екрану користувач потрапляє в Trainings Tab

![Design](https://github.com/AntonStroi/QA-Hackathon/blob/main/Requirements%20analysis%20/1.png)

- В табі Trainings новий блок: Today’s Activity, в якому знаходяться від 1 до 3 рекомендованих тренувань, в залежності від кількості обраних користувачем activity на відповідному екрані

![Design](https://github.com/AntonStroi/QA-Hackathon/blob/main/Requirements%20analysis%20/2.png)

- Title - “Recommended for you”. Subtitle - “Get daily workouts tailored to your goal and interests in [Chosen Activity #1], [#2] and [#3].”

- Якщо активності обрані тільки 2, пишемо 2, якщо тільки одна то відповідно пишемо interest (без множини): “Get daily workouts tailored to your goal and interest in [Chosen Activity #1].”

![Design](https://github.com/AntonStroi/QA-Hackathon/blob/main/Requirements%20analysis%20/3.png)

- Якщо користувач обрав 2 і більше рекомендованих activity
   - При виконані 1 з них ми замінюємо Subtitle: “Great job! [N] more workout left” 
   
   ![Design](https://github.com/AntonStroi/QA-Hackathon/blob/main/Requirements%20analysis%20/4.png)

   - При виконані всіх ми замінюємо Subtitle: “All workouts done! For an extra challenge, check out the workout library below”
   
   ![Design](https://github.com/AntonStroi/QA-Hackathon/blob/main/Requirements%20analysis%20/5.png)

   - На екрані Personal plan відмічаємо картку Do Your Workout як виконану.
- Вся область карточки клікабельна та переводить на Workout preview screen

- ***Нотатка до завдання:*** Дизайн екрану з вибором activity

 ![Design](https://github.com/AntonStroi/QA-Hackathon/blob/main/Requirements%20analysis%20/6.jpeg)

Рішення залити на github у папку ***Requirements analysis.*** В README написати тест кейси або тест кейси до задачі.

---

# Help guide
- Додаток можна завантажити за посиланням [Better Me](https://play.google.com/store/apps/details?id=com.gen.workoutme&hl=en)

- Як створити репозиторій і залити туди рішення: [GitHub Docs](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

---

# Успіхів!

---