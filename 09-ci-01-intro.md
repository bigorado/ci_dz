Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:

1. Open -> On reproduce.
2. On reproduce -> Open, Done reproduce.
3. Done reproduce -> On fix.
4. On fix -> On reproduce, Done fix.
5. Done fix -> On test.
6. On test -> On fix, Done.
7. Done -> Closed, Open.

Остальные задачи должны проходить по упрощённому workflow:

1. Open -> On develop.
2. On develop -> Open, Done develop.
3. Done develop -> On test.
4. On test -> On develop, Done.
5. Done -> Closed, Open.



<p align="center">
  <img width="831" height="580" src="./image/1.jpg">
</p>

<p align="center">
  <img width="754" height="448" src="./image/2.jpg">
</p>

<p align="center">
  <img width="1613" height="555" src="./image/3.jpg">
</p>

1) [Bugs.xml](https://github.com/bigorado/ci_dz/blob/main/files/Bugs.xml)

2) [AllTasks.xml](https://github.com/bigorado/ci_dz/blob/main/files/AllTasks.xml)