# Perseus
## CLI утилита для проведения нагрузочного тестирования и генерации сетевых запросов
Проект начат **29.05.2022** и на текущий момент **30.05.2022** эта утилита может пока что слать только HTTP запросы с методом GET.

### Как это работает?
Все очень просто вы создаете файл формата **.json** и описываете следующие поля:
1. **URL** - адрес сервера
2. **Requests** - количество запросов
3. **Pacing** - время в миллисекундах за которое гарантированно выполнится запрос, следующие запросы будут ждать окончания **pacing**

![image](https://user-images.githubusercontent.com/67442103/170935075-1398b4e1-d720-4da7-9085-2bb84153322e.png)

Далее вы запускаете утилиту командой **perseus run -f yourJsonFile.json**

![image](https://user-images.githubusercontent.com/67442103/170933715-fdec07a0-0744-432f-ba22-d363f417e6a4.png)

