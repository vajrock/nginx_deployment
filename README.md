# nginx_deployment

В даном репозитории находится решение к тестовой задаче. Название компании и позиции не публикую в публичном репозитории

Формирование нагрузки:
kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://nginx-80-port; done"

