## Развертывание Threat intelligence Platform OpenCTI

Яковлев Александр

## Цель работы

1. Освоить базовые подходы процессов Threat Intelligence

2. Освоить современные инструменты развертывания контейнеризованных приложений

3. Получить навыки поиска информации об угрозах ИБ

## Ход выполнения практической работы

Для разворачивания системы threat intelligence OpenCTI была использована система контейнеризации приложений Docker.

## Шаг 1 - Предварительная конфигурация
1. Для работы ElasticSearch требуется увеличить размер виртуальной памяти системы:

```
sudo sysctl -w vm.max_map_count=262144
```

2. Шаг 2 - Создание docker-compose.yml и .env

Был скачан и отредактирован файл по ссылке: https://github.com/OpenCTI-Platform/docker

3. Шаг 3 - Разворачиваем сервис с помощью команды:

```
docker-compose up 
```
![image](https://github.com/Marshallmeow/protectsystem/assets/89981827/38f4a0e1-0f2c-4e56-a77a-0e6e7b9f2f3d)

4. Шаг 4 - Использование системы threat intelligence OpenCTI

![image](https://github.com/Marshallmeow/protectsystem/assets/89981827/162da38a-ca6c-427e-9473-3afaa788d1ab)

1. После перехода на веб-ресурс OpenCTI пользователя встречает поле авторизации:

2. Входим по указанным в конфигурации окружения логину и паролю.

3. После входа появляется веб-интерфейс:

![image](https://github.com/Marshallmeow/protectsystem/assets/89981827/887b2d26-1434-4002-8011-b163510ab9dc)

## Оценка результата

Таким образом, были изучены возможности работы с платформой threat intelligence OpenCTI.

## Выводы

Таким образом, были изучены возможности работы с платформой threat intelligence OpenCTI.
