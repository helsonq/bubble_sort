def bubble_sort(arr):
n = len(arr)
for i in range(n):
swapped = False
for j in range(0, n-i-1):
if arr[j] > arr[j+1]:
arr[j], arr[j+1] = arr[j+1], arr[j]  # Меняем элементы местами
swapped = True
if not swapped:  # Оптимизация: выход если сортировка завершена
break
return arr


# Пример использования
example = [64, 34, 25, 12, 22, 11, 90]
print("Исходный массив:", example)
print("Отсортированный массив:", bubble_sort(example.copy()))
