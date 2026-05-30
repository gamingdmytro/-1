1. Привітання з ім'ям та віком
2. name = input("Введіть ваше ім'я: ").strip()
age = input("Введіть ваш вік: ").strip()
print(f"Привіт {name}, тобі {age}!")

2. Перевірка віку
3. age = int(input("Введіть ваш вік: ").strip())
if age > 18:
    print("Вхід дозволено!")
else:
    print("Вхід заборонено!")

3. Гра "Вгадай число"
4. import random

secret = random.randint(1, 10)
attempts = 3

for attempt in range(attempts):
    guess = int(input(f"Спроба {attempt + 1}/{attempts}. Введіть число від 1 до 10: ").strip())
    if guess == secret:
        print(f"Вітаю! Ви вгадали число {secret}!")
        break
    elif guess > secret:
        print("Менше")
    else:
        print("Більше")
else:
    print(f"На жаль, ви не вгадали. Загадане число: {secret}")

4. Виведення чисел у діапазоні
5. start = int(input("Введіть число *від*: ").strip())
end = int(input("Введіть число *до*: ").strip())

for i in range(start, end + 1):
    print(i, end=" ")
print()

5. Парні числа від 1 до n у зворотному порядку
6. n = int(input("Введіть число n: ").strip())

for i in range(n, 1, -1):
    if i % 2 == 0:
        print(i, end=" ")
print()

6. Факторіал числа
7. n = int(input("Введіть число: ").strip())
factorial = 1

for i in range(1, n + 1):
    factorial *= i

print(f"!{n} = {factorial}")

7. Визначення оцінки за балами
8. score = int(input("Введіть кількість балів (0-100): ").strip())

if score > 100 or score < 0:
    print("Некоректне значення")
elif score >= 90:
    print("Оцінка: відмінно")
elif score >= 70:
    print("Оцінка: добре")
elif score >= 50:
    print("Оцінка: задовільно")
else:
    print("Оцінка: незадовільно")

8. Калькулятор
9. a = float(input("Введіть перше число (a): ").strip())
b = float(input("Введіть друге число (b): ").strip())
operation = input("Введіть дію (+, -, *, /): ").strip()

if operation == "+":
    print(f"Результат: {a + b}")
elif operation == "-":
    print(f"Результат: {a - b}")
elif operation == "*":
    print(f"Результат: {a * b}")
elif operation == "/":
    if b == 0:
        print("Ділення на нуль")
    else:
        print(f"Результат: {a / b}")
else:
    print("Некоректна дія")
   
