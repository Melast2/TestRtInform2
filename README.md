def countElements(list) {
    // Используем метод countBy, который подсчитывает количество каждого элемента
    def result = list.countBy { it }
    
    // Возвращаем результат
    return result
}

// Пример использования
def array = [1, 3, 4, 5, 1, 5, 4]

def result = countElements(array)

// Выводим результат
result.each { key, value ->
    println "$key : $value"
}

1 : 2
3 : 1
4 : 2
5 : 2

Я проверил этот код через groovy console на android studio, он работает корректно , из-за больших проблем с интернетом в Казани не могу установить компилятор для груви 
