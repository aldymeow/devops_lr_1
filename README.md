# Отчёт по лабораторной работе №1  
## Работа с Docker, Dockerfile и Docker Compose  

**Выполнил:** Ширинкин Тимофей

**Группа:** ПИ-430Б  

---

## Ход выполнения работы

### 1. Изучение теоретической части  
Были изучены:  
- основные команды Docker;  
- структура Dockerfile;  
- назначение Docker Compose.  

### 2. Установка Docker Desktop  
На компьютер установлен Docker Desktop, содержащий Docker Engine и Docker Compose.  

<img width="1898" height="992" alt="511656075-a90736d9-bc0d-4561-a694-5855c4416316" src="https://github.com/user-attachments/assets/b3604236-7649-4127-9387-16478f450666" />


### 3. Создание проекта Flask  
В рабочей директории созданы файлы:  
- `app.py`  
- `requirements.txt`

<img width="1046" height="756" alt="511656128-46ef2c03-6ba0-443e-b01a-2c3d474ffc32" src="https://github.com/user-attachments/assets/a5c5ac56-8275-448e-88bf-b0482c246b49" />

 <img width="352" height="92" alt="511656142-a90ae7a2-567b-4eeb-bf7d-7e0ed85c0d1b" src="https://github.com/user-attachments/assets/7feb55a4-08a6-4a3c-a223-09e05303bed7" />


### 4. Создание Dockerfile  
Создан Dockerfile для сборки образа приложения.  

<img width="672" height="382" alt="511656220-af43c25a-7435-4d76-ba44-56a645d04d55" src="https://github.com/user-attachments/assets/319ee5c4-84d2-4b4f-b28c-16d765cfc44f" />

### 5. Создание docker-compose.yml  
Создан файл `docker-compose.yml`.  

<img width="775" height="836" alt="11" src="https://github.com/user-attachments/assets/ed9ec9aa-3424-4e19-a6c7-b7e10f4f6f09" />



### 6. Запуск  
Образ собран командой: docker build -t myapp:1.0 . Прописываем docker compose up --build. Первая часть команды запускает все сервисы, создаёт контенеры, а вторая - пересобирает все образы прописанные в build: 

<img width="1038" height="202" alt="22" src="https://github.com/user-attachments/assets/4b1c662b-8c7a-49cf-b3c7-740c90ac0963" />

### 7. Открываем localhost  

<img width="1043" height="225" alt="33" src="https://github.com/user-attachments/assets/c6585d39-0e3b-49c9-b44d-b7ee91d63b04" />

### Заключение 
В ходе лабораторной работы были изучены команды Docker и Docker Compose, созданы и запущены контейнеры Flask и PostgreSQL.
Были решены конфликты портов и ошибки аутентификации.

В результате:  
- Flask-приложение успешно подключено к PostgreSQL;
- Получен практический опыт сборки образов и запуска многосервисных приложений через Docker Compose;
- Освоены методы отладки контейнеров и проброса портов.

Работа показала эффективность Docker для развёртывания переносимых приложений.
