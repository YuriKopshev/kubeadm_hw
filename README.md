# Домашнее задание к занятию "`Установка Kubernetes`"

## Результаты установки кластера Kubernetes из 5 нод

## Конфигурация кластера
Кластер развернут методом K8s-in-Docker (kind), симулирующим Ubuntu-узлы.

*   **Количество нод:** 5 (1 Master, 4 Workers)
*   **CRI:** containerd
*   **etcd:** Запущен на Master-ноде

## Подтверждение выполнения
1. Список нод кластера и CRI: `kubectl get nodes -o wide` 

![скриншот 1]()

2. Расположение etcd: `kubectl get pods -n kube-system -l component=etcd -o wide` 

![скриншот2]()
