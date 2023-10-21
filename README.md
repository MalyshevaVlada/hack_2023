# axenix_mov
Команда: CoffeeDose
Кейс: Мониторинг автоматизированного склада
![Дизайн без названия (5)](https://github.com/NastyaZiss/hack_2023/assets/88962864/f2cc826d-a411-4b58-a701-d12087d9daeb)

![image](https://github.com/NastyaZiss/hack_2023/assets/88962864/bd433170-359f-48e5-827c-b8501af93c08)

![image](https://github.com/NastyaZiss/hack_2023/assets/88962864/30c1783a-8dfb-447d-bd0e-8881e358093f)


1) получение данных  из скрипта и имитация движения погрузчиков (с сохранением в БД)
2) передача данных о погрузчиках через сокеты, остальные данные через http

Стек: fastapi, sqlalchemy, python, postgresql, docker

![image](https://github.com/NastyaZiss/hack_2023/assets/88962864/3912d6f9-116c-4256-8b4d-bc4cf757af42)

4) панель для отображения данных о:
  - погрузчиках ( идентификатор, статус, номер заказа, последнее ТО, следующее ТО)
  - контрольных точек* (общее количество проходов, количество проходов определённого погрузчика)
  - заказов* (идентификатор, статус заказа, номер погрузчика, время выполнения)
  - выходе из строя контрольной точки*
(данные открываются по клику на объект на схеме)




![image](https://github.com/NastyaZiss/hack_2023/assets/88962864/b831cddf-df49-4487-95d7-83480b7dfb26)

  - выбор погрузчика (определённый или все)
  - выбор промежутка времени
  - пройденное расстояние
  - выполненные заказы
  - время проведённое в движении
  - время нахождения в каждом из статусов (ожидание, поездка до заказа, возвращение с заказом)
  - реализованно в виде таблиц

* - дополнительные задачи
