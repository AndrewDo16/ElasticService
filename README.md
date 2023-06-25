# ElasticService

Проект Spring Elastic представляет собой веб-приложение, основанное на фреймворке Spring Boot и интегрированное с Elasticsearch. 

# Требования
Перед запуском проекта убедитесь, что у вас установлены следующие компоненты:
 • Docker: для развертывания и управления контейнерами

# Установка и запуск
  Склонируйте репозиторий проекта на свою локальную машину.
  Перейдите в корневую директорию проекта.
  Запустите контейнер Elasticsearch с помощью команды:

  docker-compose up -d

  Это запустит контейнер Elasticsearch и контейнер WebService и настроит их для дальнейшей работы.

  
# Использование API

 • POST /catalog/import - Импорт каталога по URL. Пример: https://front-end.tanuki.ru/feeds/tanuki/voronezh
 
 • GET / - Получить список всех продуктов.
 
 • GET /products/ - Получение списка продуктов (один метод)с возможностью полнотекстового поиска по полю nameи и фильтрация по categoryId (возможно не указывать параметр categoryId)


# Дополнительная информация
 • Вся конфигурация приложения находится в файлах docker-compose.yaml и Dockerfile.
