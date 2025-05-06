# Лабораторная работа №3 «Разработка инфраструктуры MVP AI приложения.»  
University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FTMI](https://itmo.ru/ru/viewfaculty/87/fakultet_tehnologicheskogo_menedzhmenta_i_innovaciy.htm)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)  
Year: 2024/2025  
Group: U4125  
Author: Tsvirko Elina Vitalievna  
Lab: Lab4  
Date of create: 05.05.2025  
Date of finished:    
## Начальное состояние:  
Для MVP необходимо недорогое решение с минимальным функционалом    
Frontend и Backend развертываются на Cloud Run.  
Для БД и ее хранения я взяла Firestore и Cloud storage соответственно. На начальном этапе Firestore берем NoSQL.   
  
![1](/img/4.1.1.png)  
  
Стоимость:  

![1](/img/4.1.png)    
  
## Тестирование партнерами:  
На данном этапе происходит расширение функционала предыдущей схемы. Меняются входящие требования для нагрузки системы и ее функционала.  
Для отслеживания ошибок и метрик добавляется Cloud Monitoring   
  
  
![1](/img/4.2.2.png)  
  
Стоимость:  

![1](/img/4.2.png)    
  
## Продовое решение:    
Вместо Cloud Run теперь используем Google Kubernetes, который позволяет масштабировать систему, распределять нагрузку системы, обеспечивая ее отказоустойчивость.  
Firestore заменяем на Cloud SQL, так как подразумеваем сильно больший объем данных, тем самым облегчая работу с БД. Для отслеживания большего количества метрик используем Cloud Operations Suite.  
Как и в предыдущем пункте, меняем входящие требования к системе.    
  
![1](/img/4.3.3.png)  
  
Стоимость:  

![1](/img/4.3.png)
