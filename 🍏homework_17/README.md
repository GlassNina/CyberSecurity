## Домашнее задание № 17  
### Защита инфраструктуры приложений  
#### virtualization, cloud, containers  

### 1. Исследуем docker  
#### ●	Скачать образ ubuntu:18.04 c hub.docker.io, проверить целостность и соответствие контрольной суммы образа SHA256  
![Homework_17_01.jpg](Homework_17_01.jpg)  
![Homework_17_02.jpg](Homework_17_02.jpg)  
![Homework_17_03.jpg](Homework_17_03.jpg)  
#### ●	С помощью команды docker image ls отобразить все docker образы на системе, добавить в группу docker вашего пользователя для запуска команд docker без sudo  
![Homework_17_04.jpg](Homework_17_04.jpg)   
#### ●	Запустить данный образ в интерактивном режиме в оболочке sh docker run -it <image name> sh  
![Homework_17_05.jpg](Homework_17_05.jpg)   
![Homework_17_06.jpg](Homework_17_06.jpg)   
#### ●	Внутри контейнера выполнить команду whoami для определения пользователя под которым вы запустили контейнер  
![Homework_17_07.jpg](Homework_17_07.jpg)   
#### ●	Запустить контейнер под пользователем tms  
#### ●	Прогнать образ через один из сканеров безопасности проанализировать результаты:  
#### ●	https://github.com/quay/clair  
#### ●	https://github.com/aquasecurity/trivy  
![Homework_17_08.jpg](Homework_17_08.jpg)   
![Homework_17_09.jpg](Homework_17_09.jpg)   

### *2. Пишем Dockerfile    
#### ●	Скачать и видоизменить файл конфигурации nginx.conf, файл должен выводить “Welcome to the TMS Cybersecurity Course”    
![Homework_17_10.jpg](Homework_17_10.jpg)   
![Homework_17_11.jpg](Homework_17_11.jpg)   
#### ●	Создать Dockerfile c базовым образом ubuntu:20.04, в котором вы устанавливаете Nginx веб сервер, а затем копируете заранее скачанный файл конфигурации nginx.conf во внутрь директории nginx контейнера    
![Homework_17_12.jpg](Homework_17_12.jpg)   
![Homework_17_13.jpg](Homework_17_13.jpg)     
#### ●	Запускаем контейнер перебрасывая 8800 порт хоста на 80 порт контейнера    
![Homework_17_14.jpg](Homework_17_14.jpg)     
![Homework_17_15.jpg](Homework_17_15.jpg)   
![Homework_17_16.jpg](Homework_17_16.jpg)   
![Homework_17_17.jpg](Homework_17_17.jpg)   
#### ●	Вывод 127.0.0.1:8800 в браузере скриним      
![Homework_17_18.jpg](Homework_17_18.jpg)   