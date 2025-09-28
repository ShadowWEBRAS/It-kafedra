# Laravel API

### API:
- Авторизация через Laravel Sanctum.
- Методы для регистрации, авторизации и работы с корзиной, товарами 

## Требования

- PHP 8.1 или выше
- Composer
- MySQL 8.0 или выше
- Laravel 10
- Postman (для тестирования API)

---
Я пробовал настроить Docker но не получилось, удалять из проекта не стал. Также некоторые endpoints не работают или могут работать не совсем корректно
---

## Установка

git clone https://github.com/ShadowWEBRAS/It-kafedra.git 

cd It-kafedra\project

cp .env.example .env

mkdir -p bootstrap/cache
mkdir storage\framework\sessions
mkdir storage\framework\views
mkdir storage\framework\cache

composer update

php artisan package:discover --ansi

php artisan key:generate

php artisan migrate

php artisan serve

Тестирование запросов через postman

подробней в самой коллекции а здесь я кратко расскажу какие запросы можно отправлять

POST:
На регистрацию
На вход
На создание товара
GET:
Получение товара


