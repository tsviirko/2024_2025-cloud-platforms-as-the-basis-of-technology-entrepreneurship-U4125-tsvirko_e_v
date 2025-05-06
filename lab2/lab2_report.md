# Лабораторная работа №2 «Исследование Cloud Run»  
University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FTMI](https://itmo.ru/ru/viewfaculty/87/fakultet_tehnologicheskogo_menedzhmenta_i_innovaciy.htm)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)  
Year: 2024/2025  
Group: U4125  
Author: Tsvirko Elina Vitalievna  
Lab: Lab2  
Date of create: 29.04.2025  
Date of finished: 05.05.2025  
  
## Ход работы  
## Создание сервиса Cloud Run  
В Google cloud я зашла в раздел Cloud Run и создала дефолтный сервис Hello, не меняя параметры.   
Переход по ссылке доказал, что сервис был успешно создан, что также подтверждает лог (статус GET 200)
![1](/img/2.1.jpg)  
  
## Логи и метрики  
Лог, скриншот которого представлен выше, показывает ход создания сервиса, когда и кем он создавался и, в данном случае, успех создания.
  
В метриках мы видим различные графики.  
![2](/img/2.2.jpg)  
![3](/img/2.3.jpg)  
![4](/img/2.4.jpg)   
![5](/img/2.5.jpg)

## Смена порта Cloud Run и переключение трафика  
Я зашла в настройки и поменяла порт с 8080 на 8090.  
Сервис был успешно запущен. 
Далее я меняла трафик в следующих соотношениях 50/50, 5/95 и 80/20.  
На следующих графиках представлены метрики для 4 состояний сервиса, где 1 засечка - изменение порта, 2,3,4 - изменение трафика в разных пропорциях
![6](/img/2.6.jpg)  
![7](/img/2.7.jpg)   
![8](/img/2.8.jpg)  
![9](/img/2.9.jpg)  
![10](/img/2.10.jpg)  
![11](/img/2.11.jpg)  
  
## Удаление ресурсов  
Все созданные ресурсы по окончанию работы удалила.
