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

