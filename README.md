# Тестовое задание для DevOps
# 🎯 Цель

Оценить способность кандидата самостоятельно выстроить полный цикл CI/CD, включая:
	•	автоматическую сборку и тестирование,
	•	контейнеризацию,
	•	деплой,
	•	мониторинг и логирование,
	•	реализацию rollback-стратегий.

# Sausage Store

![image](https://user-images.githubusercontent.com/9394918/121517767-69db8a80-c9f8-11eb-835a-e98ca07fd995.png)


## Technologies used

* Frontend – TypeScript, Angular.
* Backend  – Java 16, Spring Boot, Spring Data.
* Database – H2.

## Installation guide
### Backend

Install Java 16 and maven and run:

```bash
cd backend
mvn package
cd target
java -jar sausage-store-0.0.1-SNAPSHOT.jar
```

### Frontend

Install NodeJS and npm on your computer and run:

```bash
cd frontend
npm install
npm run build
npm install -g http-server
sudo http-server ./dist/frontend/ -p 80 --proxy http://localhost:8080
```

Then open your browser and go to [http://localhost](http://localhost)

# ✅ Задачи

## 1. Контейнеризация
	•	Создать Dockerfile для фронтенда и бэкенда.
	•	Настроить docker-compose.yml для совместного запуска компонентов.
	•	Обеспечить возможность запуска приложения одной командой.

## 2. CI
	•	Настроить CI-пайплайн (например, GitHub Actions), который:
	•	собирает и тестирует фронтенд и бэкенд,

## 3. Мониторинг и логирование
	•	Интегрировать Prometheus для сбора метрик с бэкенда.
	•	Настроить Grafana для визуализации метрик.
	•	Настроить централизованное логирование (например, с использованием ELK-стека или Loki).

## 4. Документация
	•	Подготовить README.md с инструкциями по:
	•	сборке и запуску приложения,
	•	работе CI пайплайна,
	•	настройке мониторинга и логирования,
# 📬 Формат сдачи
Публичный GitHub репозиторий с реализованными задачами (можно сделать fork от этого репозитория).
