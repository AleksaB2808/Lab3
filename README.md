# Lab3
Функція task1


def task1(my_list):
    my_list.insert(1, -5)

    min_element = min(my_list)
    max_element = max(my_list)

    my_list.insert(2, [1, 2, 3])

    my_list.append(["Проценко", "Ярослав"])

    list_length = len(my_list)

    print("my_list:", my_list)
    print("min_element:", min_element)
    print("max_element:", max_element)
    print("list_length:", list_length)

    return my_list, min_element, max_element, list_length
Опис:

my_list.insert(1, -5): Вставляє число -5 на позицію з індексом 1 у вхідний список my_list.
min_element = min(my_list): Знаходить мінімальний елемент у списку my_list.
max_element = max(my_list): Знаходить максимальний елемент у списку my_list.
my_list.insert(2, [1, 2, 3]): Вставляє список [1, 2, 3] на позицію з індексом 2 у вхідний список my_list.
my_list.append(["Проценко", "Ярослав"]): Додає список ["Проценко", "Ярослав"] в кінець вхідного списку my_list.
list_length = len(my_list): Знаходить довжину (кількість елементів) списку my_list.
При друкуванні виводяться значення my_list, min_element, max_element та list_length.
Повертається кортеж з вхідним списком my_list, мінімальним і максимальним елементами і довжиною списку my_list.
Функція task2

def task2(A, B, C):
    total_cost = sum([quantity * price for quantity, price in zip(B, C)])
    average_price = sum(C) / len(C)
    most_stocked_index = B.index(max(B))
    most_stocked_item = A[most_stocked_index]
    return total_cost, average_price, most_stocked_item
Опис:

total_cost = sum([quantity * price for quantity, price in zip(B, C)]): Обчислює загальну вартість товарів, перемножаючи кількість (quantity) на ціну (price) для кожної пари зі списків B і C.
average_price = sum(C) / len(C): Обчислює середню ціну товарів у списку C, діливши суму всіх цін на їх кількість.
most_stocked_index = B.index(max(B)): Знаходить індекс товару з найбільшою кількістю на складі в списку B.
most_stocked_item = A[most_stocked_index]: Знаходить найбільш на складі товар, використовуючи індекс most_stocked_index у списку A.
Повертається кортеж із значень total_cost, average_price та most_stocked_item.
Функція task3

def task3():
    # Сформуємо список із 50 елементів в діапазоні від -25 до 25
    my_list = list(range(-25, 26))

    A1 = []
    A2 = []

    for i in my_list:
        if i > 0:
            A1.append(i)
        else:
            A2.append(i)
    return A1, A2
Опис:

Створюється список my_list, що містить числа від -25 до 25.
Ініціалізуються порожні списки A1 і A2.
Проходиться по кожному елементу i у списку my_list.
Якщо i більше 0, то додається до списку A1.
Інакше i додається до списку A2.
Повертається кортеж із списків A1 і A2, що містять відповідно всі позитивні та від'ємні числа зі списку my_list.
Ці функції виконують вказані операції та повертають результати відповідно до вхідних параметрів та завдань, описаних у коді.
