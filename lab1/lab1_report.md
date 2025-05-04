# Лабораторная работа №1 «Обзор Google Cloud и исследование основных сервисов»  
University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FTMI](https://itmo.ru/ru/viewfaculty/87/fakultet_tehnologicheskogo_menedzhmenta_i_innovaciy.htm)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)  
Year: 2024/2025  
Group: U4125  
Author: Tsvirko Elina Vitalievna  
Lab: Lab1  
Date of create: 04.05.2025  
Date of finished:  
## Ход работы  
## Создание виртуальной машины  
В разделе IAM & Admin — Service Account и создала аккаунт с ролью Storage Admin.   Затем, я создала виртуальную машину во вкладке Compute Engine с Machine type e2-micro, во вкладке Advanced выбрала режим Spot.   
Также для успешного выполнения работы, до запуска ВМ, был изменен в настройках машины аккаунт с дефолтного на созданный раннее.   
Здесь нет скриншотов, потому что я не подумала сделать их по всему ходу работы.
  
Подключение к машине выполнялось через SSH-ключ.

## Выполнение основной части задания   
С помощью утилиты gsutils был найден необходимый бакет lab1-bucket-itmo. Далее мы копировалие 3 файла. С помощью команды ls -lah видно, что эти файлы теперь хранятся на моей ВМ.
![1](/img/photo_5238179820175749450_x.jpg)
  
## Смена роли на Compute Viewer  
В режиме редактирования, во вкладке Service Account, я установила новую роль —  Compute Viewer.  
Аналогично предыдущему пункту, пробовала повторить все предыдущие действия, но уже на моменте поиска бакета мы видим ошибку AccessDeniedException 403, говорящую о недостаке прав.  
![2](/img/photo_5237829041606751157_y.jpg)
  
## Удаление ресурсов  
В конце работы я все удалила.
