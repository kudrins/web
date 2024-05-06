## Домашнее задание Развертывание веб приложения

### Описание домашнего задания
```
- создать стенд с рабочими веб-приложениями в 3 разных стеках:
  nginx + php-fpm (wordpress) + python (django) + js (node.js)
- веб-приложения устанавливаются через docker-compose 
- VM разворачивается в среде VMware vSphere 7 из шаблона Centos 8 Stream
  
Приложения развернуты в контейнерах docker

Файлы:

- network.yml:                ansible playbook развертывания и настройки VM
- vars.yml:                   переменные для создания и натройки VM
- host:                       inventory

- docker-compose.yml:         сценарий развертывания контейнеров docker с приложениями
- .env:                       файл переменных создания и подключения БД и веб-приложения
- nginx-conf/nginx.conf:      файл конфигурации nginx
- node/test.js:               файл node.js приложения
файлы настройки веб-приложения django:
- python/Dockerfile          
- python/manage.py           
- python/requirements.txt   
- python/mysite/settings.py  
- python/mysite/urls.py      
- python/mysite/wsgi.py      

 Результаты проверки в скриншотах:
- screens\ansible.jpg:        работа ansible-playbook
- screens\docker.jpg:         контейнеры docker
- screens\8081.jpg:           веб-приложение django
- screens\8082jpg:            веб-приложение node.js
- screens\8083jpg:            веб-приложение wordpress

 
