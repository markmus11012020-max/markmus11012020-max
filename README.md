# 👋 Приветствую! Я Гульназ Мусина — AI-разработчик & Инженер генеративного ИИ

Управленец с 23-летним бэкграундом и эксперт в области AI-автоматизации. Совмещаю понимание бизнес-процессов с вайб-кодингом и Prompt Engineering. Фокус — проектирование ИИ-агентов и быстрое создание масштабируемых MVP.

---

## 🛠 Мой технологический стек & AI-компетенции

- **AI & Prompt Engineering:** Prompt Chaining, Agentic AI, RAG (Metadata-Driven), оптимизация контекста LLM (Token Economy), работа в Cursor / Cline, модели OpenAI, Anthropic, DeepSeek, YandexGPT, GigaChat.
- **Backend-разработка:** Java 17, Spring Boot 3.x, Spring Data JPA (Hibernate), PostgreSQL 15, REST API, Maven; Python, FastAPI, SQLAlchemy (async), Pydantic v2, Alembic, SQLite; TypeScript, C#.
- **Инфраструктура и DevOps:** Docker, Docker Compose, Git, Yandex Cloud (Ubuntu VM), скрипты CI/CD-автодеплоя, логирование и мониторинг.
- **Комплаенс и безопасность:** ФЗ-152 (персональные данные), ФЗ-115 (AML), локальная анонимизация/токенизация данных, суверенные LLM-провайдеры.
- **Управление:** Product Ownership, системный анализ, руководство командами, техническая документация.

---

## 🚀 Ключевые AI-проекты (Live MVPs)

### 1. FinTech Compliance AI-Orchestrator — Java / Spring Boot · Live MVP

> Production-ready микросервис AML-комплаенса для российского финтеха и банков: ИИ-агент проводит скоринг подозрительных транзакций с полным соблюдением **ФЗ-115** и **ФЗ-152**.

- **Стек:** Java 17, Spring Boot 3.2.5, Spring Data JPA + Hibernate, PostgreSQL 15, Spring RestTemplate, Docker / Docker Compose, Yandex Cloud.
- **Архитектура (ООП):** паттерн **Strategy** (`LlmProvider` → mock / YandexGPT / GigaChat), **Factory** (`LlmProviderFactory` с graceful fallback), **Repository** (`AuditLogRepository`), Dependency Injection через Spring-контейнер.
- **Пайплайн:** Анонимизация ПДн → вызов суверенной LLM → деанонимизация отчёта. Карта замен хранится только в памяти JVM, в аудит-лог попадают лишь метаданные.
- **Эндпоинты:** `POST /api/v1/compliance/check`, `POST /api/v1/compliance/check-raw`, `GET /api/v1/compliance/info`, `GET /api/v1/health`.
- 🔗 Исходный код: [github.com/markmus11012020-max/FinTech-Compliance-AI-Orchestrator](https://github.com/markmus11012020-max/FinTech-Compliance-AI-Orchestrator)
- 🟢 Живое демо (Swagger UI / OpenAPI): **http://158.160.152.145:8080/swagger-ui.html** · спецификация: http://158.160.152.145:8080/api-docs

### 2. Helpdesk AI Backend — Python / FastAPI · Live MVP

> Асинхронный ИИ-сервис классификации и маршрутизации обращений. B2B Enterprise ready · ФЗ-152 · PostgreSQL · YandexGPT / GigaChat.

- **Функции:** асинхронный триаж обращений (`POST /api/v1/tickets/triage`), 4 категории (`billing`, `support`, `complaint`, `other`), уровни уверенности с автоэскалацией, API-key guard, rate limiting, fail-safe fallback при сбое LLM.
- 🔗 Исходный код: [github.com/markmus11012020-max/helpdesk-ai-backend](https://github.com/markmus11012020-max/helpdesk-ai-backend)
- 🟢 Живое демо (Live API / Swagger UI): **http://158.160.152.145:8000/docs**

### 3. Universal AI SQL Assistant — Python · Metadata-Driven RAG

> ИИ-ассистент генерации enterprise-level SQL (PostgreSQL) по бизнес-требованиям на естественном языке. Динамический Context Injection из `app_metadata.json`, ультра-экономная Token Economy (Prompt Caching, Stop Sequences), строгий DWH-валидатор UPPERCASE / `UPPER()`.
- 🔗 [github.com/markmus11012020-max/universal-ai-sql-assistant](https://github.com/markmus11012020-max/universal-ai-sql-assistant)

### 4. AI Client Report Generator — Python · Автоматизация документов

> Сквозная генерация PDF-отчётов с помощью LLM и HTML-шаблонов: отчёт по диалогу с клиентом, бриф на дизайн сайта, карточка товара для маркетплейса. Стек: Flask, Jinja2, WeasyPrint, Pillow.
- 🔗 [github.com/markmus11012020-max/AI-Client-Report-Generator](https://github.com/markmus11012020-max/AI-Client-Report-Generator)

### 5. Lead Intake Service — FastAPI · MVP

> Прототип сервиса приёма и логирования заявок (лидов) с валидацией данных и сохранением в SQLite; интерактивная документация Swagger UI.
- 🔗 [github.com/markmus11012020-max/MVP_lead-intake-service](https://github.com/markmus11012020-max/MVP_lead-intake-service)

### 6. Telegram AI-агенты и VK-боты — Python

> Асинхронные боты с управлением сессиями и токенами: ИИ-боты на GPT, бот-резюме для HR-скрининга, туристический VK-бот, бот погоды.
- 🔗 [TG-BOT-GPT](https://github.com/markmus11012020-max/TG-BOT-GPT) · [Resume-TG-bot](https://github.com/markmus11012020-max/Resume-TG-bot) · [vk-bot-travel-agent](https://github.com/markmus11012020-max/vk-bot-travel-agent)

---

## 🎓 Образование и квалификация

- **РАНХиГС** (Июль 2026): Удостоверение о повышении квалификации по программе *«Специалист по ИИ-инструментам: запросы и автоматизация без кода»*.
- **ZeroCoder**: Курс «Промт-инженер / вайб-кодер», сентябрь 2026.
- **СГЭА (Самара)**: Высшее экономическое образование (Экономическая теория, Организация рынка ценных бумаг).
- **ФСФР**: Серия 2.0 — сертификат.

---

## 📬 Контакты для связи

- 📱 **Телефон / Telegram:** +7 (962) 609-00-01 / [@GulnazM1101](https://t.me/GulnazM1101)
- 📧 **Email:** gmusina@list.ru
- 📍 **Локация:** Самара (готова к удаленной работе или офису)
