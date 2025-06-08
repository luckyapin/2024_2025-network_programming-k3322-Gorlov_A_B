University: [ITMO University](https://itmo.ru/ru/)

Faculty: [PIN](https://fict.itmo.ru)

Course: [Introduction in routing](https://github.com/itmo-ict-faculty/introduction-in-routing)

Year: 2024/2025

Group: K3322

Author: Gorlov Andrey Borisovich

Lab: [Lab3]([https://itmo-ict-faculty.github.io/network-programming/education/labs2023_2024/lab2/lab2/#_5](https://itmo-ict-faculty.github.io/network-programming/education/labs2023_2024/lab3/lab3/#_5))

Date of create: 08.06.2025

Date of finished: 08.06.2025

# Настройка окружения

Скачиваем Vagrant и репозиторий
Заходим в папку vm-ubuntu-20.04, заходим в консоль и пишем 
```cmd
vagrant up
```
Ждём некоторое время и появляется виртуалка 

![image](https://github.com/user-attachments/assets/95c23106-440d-4e9a-b7bd-149895cd6e11)


# Код

Во все todo вписываем то, что необходимо и в итоге получаем готовую логику для роутера

![Файл](base.p4)

# Исправляем все ошибки

В utils/Makefile убираем pb в .txtpb
![image](https://github.com/user-attachments/assets/d0fba4d1-fc09-4320-b9ac-b7368e133e83)

Далее в triandle-pogo во всех json делаем аналогично
![image](https://github.com/user-attachments/assets/f3b33be7-8868-4b2a-802a-ead6ab578360)

В конце в файле helper.py убираем параметр allow_unknown_field=True

![image](https://github.com/user-attachments/assets/2c419b17-2508-425e-a82f-e4901233586d)


# Всё работает
Пишем в консоль sudo make run

Внутри пингуем 
![image](https://github.com/user-attachments/assets/8610ac8e-08c4-41e8-bc9c-e441edad4c6e)

![image](https://github.com/user-attachments/assets/4a57104d-56f3-48df-bdaf-62e0272a5b74)
