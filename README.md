bet = 10

# Задаем регионы Дальнего Востока
countr = str(input("В каком регионе проживаете? "))
countr_1 = ("Дальний Восток")


# Кол-во детей
child = int(input("Укажите количество детей: "))

# Зарплатный проект
sal_project = input("Есть ли зарплатный проект в  банке? Y/N: ")

# Страхование
ins = input("Оформлено ли страхование в банке? Y/N: ")

if countr == countr_1 :
  print("Ваша ставка: 2%")
else:
  if child > 3:
    bet -= 1
  if sal_project == "Y" or sal_project == "y":
    bet -= 0.5
  if ins == "Y" or ins == "y":
    bet -= 1.5
  print(bet)
