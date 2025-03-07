«Кластеризация и балансировка нагрузки»

### Задание 1

- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

[Playbook 1](https://github.com/hovhannisyan-code/cluster/blob/master/playbook-1.yml)
![Result 1](https://github.com/hovhannisyan-code/cluster/blob/master/img/screenshot_0.png)

### Задание 2

- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

[Playbook 2](https://github.com/hovhannisyan-code/cluster/blob/master/playbook-2.yml)
![Result 2](https://github.com/hovhannisyan-code/cluster/blob/master/img/screenshot_1.png)
![Result 3](https://github.com/hovhannisyan-code/cluster/blob/master/img/screenshot_2.png)
