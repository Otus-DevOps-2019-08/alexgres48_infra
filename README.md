# alexgres48_infra
alexgres48 Infra repository
#HomeWork_5 Знакомство с облачной инфраструктурой

bastion_IP = 35.240.104.69
someinternalhost_IP = 10.132.0.5

Создать config в ~/.ssh
Добавить:
Host bastion Hostname 35.240.104.69 User <appuser>
Host someinternalhost ProxyCommand ssh -q bastion nc -q0 10.132.0.5 22

Подключаемся: ssh <appuser>@someinternalhost

#######################################################################

#HomeWork_6 Основные сервисы Google Cloud Platform (GCP).

testapp_IP = 35.195.152.170
testapp_port = 9292

Выполнено:
1)Установлен sdk gcloud
2)Создан хост
3)Установлен ruby
4)Установлен mongodb (обновился ключ репо, новый добавлен в скрипт)
5)Запущено и проверено приложение
6)Созданы скрипты для каждого из этапов
