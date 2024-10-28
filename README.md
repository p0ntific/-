Научная работа

### Информация

Приложение с возможностью локального запуска или интеграции в код

Генерирует по начальным параметрам диаграму заданного размера

правила генерации:

каждая клетка c, которую можно добавить в диаграмму, дает прямоугольник, в котором эта клетка в правом верхнем углу, а клетка у начала координат -- в левом нижнем. Считаем его площадь и возводим в степень alpha и обозначим S(c), где c -- клетка, а alpha -- какой-то параметр, который для начала можно взять равным 1.  И вероятность клетки берем пропорционально S(c). То есть вероятность добавить клетку c это S(c)/sum(S(c')), где сумма берется по всем клеткам c', которые можно добавить в текущую диаграмму.Потом добавляем случайно выбранную с такими вероятностями клетку и с получившейся диаграммой повторяем то же самое.  И так много раз (скажем, 1000), чтобы заметить какую-то закономерность.


### Функциональные требования системы

Система должна предоставлять возможность задать начальные клетки диаграммы - TODO

возможность контролировать коэффициент альфа - TODO

сохранять результат в файл - сделано

предоставлять удобный интерфейс в коде для интеграции в другие приложения - сделано





