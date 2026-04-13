# Привет, я Алексей! 👋

<p align="left">
<a href="https://t.me/alezovv" target="blank"><img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white" alt="alezovv" /></a>
<a href="mailto:alezovv2523@gmail.com" target="blank"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="alezovv2523@gmail.com" /></a>
</p>

### 👨‍💻 Обо мне
* 🚀 **Backend Developer** | Go • Python • C++
* 🎓 Студент **МАИ** (Фундаментальная информатика и информационные технологии).
* ⚙️ Специализируюсь на высоконагруженных системах и автономных AI-агентах.
* 🐧 Основная ОС: **Ubuntu**, топлю за автоматизацию и эффективный софт.

---

### 🛠 Стек технологий

| Категория | Инструменты |
| :--- | :--- |
| **Языки** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat&logo=go&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat&logo=c%2B%2B&logoColor=white) |
| **Backend** | `FastAPI` `Gin` `Django` `Clean Architecture` `gRPC` |
| **Data & Messaging** | `PostgreSQL` `ClickHouse` `Redis` `RabbitMQ` `Apache Kafka` |
| **DevOps** | `Docker` `Kubernetes` `GitHub Actions` `Prometheus` `Grafana` |
| AI & LLM Ops | `RAG` `Vector Databases (pgvector)` `Semantic Search` `Ollama` `Embeddings` |
| **System Dev** | `GDB` `Valgrind` `Make/CMake` `Memory Management` `POSIX Threads` |
| **Automation** | `n8n (Self-hosted)` `Docker-first nodes` `Custom JS nodes` |

---

### 🚀 Избранные проекты

#### 🔍 Smart Procurement Service (Backend)
*Интеллектуальный сервис подбора завупок на базе семантического поиска.*
* **RAG-пайплайн:** Реализовал двухэтапный поиск: отбор Top-K кандидатов через **pgvector** → точное косинусное реранжирование через **rubert-tiny2**.
* **Особенности:** Полностью offline-решение (без внешних API), модель кэшируется внутри Docker-образа при сборке.
* **Стек:** FastAPI, PostgreSQL (pgvector), Sentence-Transformers.

#### 📈 PriceTracker API
*Бэкенд-сервис для мониторинга котировок и уведомлений.*
* **Архитектура:** Связка **Celery + Redis + Celery Beat** для периодического опроса внешних API (CoinGecko) и записи истории цен.
* **Оптимизация:** Внедрил кэширование цен в Redis с TTL для снижения нагрузки на внешние эндпоинты.
* **Стек:** FastAPI, PostgreSQL, Redis, Celery.

#### 📄 Contract Accounting API
*MVP системы учета договоров и взаиморасчетов для малого бизнеса.*
* **Функционал:** Автоматизация учета дебиторской задолженности и контроля оплат между контрагентами (физ. и юр. лица).
* **Стек:** FastAPI, SQLAlchemy, PostgreSQL.

#### 🤖 n8n HH.ru Analyzer
*Автоматизированный инструмент для анализа вакансий и рынка труда.*
* Спроектировал Low-code пайплайн в **n8n** для парсинга, фильтрации и структурирования данных с HeadHunter.

#### 📐 Rigid Body Interpolation & Simulation
*Система аппроксимации промежуточных положений твердого тела в 3D-пространстве.*
* **Математика:** Реализовал алгоритм интерполяции матриц трансформации (OpenGL World Matrix) в системе однородных координат для плавного перехода между кадрами.
* **Визуализация:** Отрисовка траекторий и состояний тела в статике и динамике (анимация движения).
* **ML Integration:** Собрал датасет положений через физические симуляторы (PyBullet/Blender) и обучил регрессионную модель для предсказания промежуточных состояний.
* **Стек:** Python (NumPy, SciPy), Matplotlib/OpenGL, PyBullet.

---

### 🎓 Опыт и обучение
* **Яндекс Лицей** — Специализация «Веб-разработка на Go».
* **Яндекс Практикум** — Backend-разработчик (Python).
* **VK Education** — Системное программирование (C/C++, Linux, Unix-like OS).
  * Изучил взаимодействие с ядром ОС, организацию файловых систем, многозадачность (IPC, многопоточность) и сетевое взаимодействие через сокеты.
  * Практика: Реализовал комплексные проекты с автопроверкой (многозадачность, IPC, файловые системы, сокеты).
---

### 🏆 Хакатоны и Интенсивы (2025-2026)

#### 🏛 RosEltorg 2026 | Интеллектуальный поиск закупок (RAG-based)
**Задача:** Автоматизация подбора тендеров под сложную номенклатурную матрицу поставщика.
* **RAG Architecture:** Реализовал **Offline RAG пайплайн** без использования внешних облачных API для безопасности данных.
  * **Retrieval:** Внедрил векторный поиск через `pgvector` для быстрого отбора релевантных документов из БД.
  * **Reranking:** Настроил двухэтапную схему (Bi-Encoder для поиска + Cross-Encoder `rubert-tiny2` для финального ранжирования), что значительно повысило точность выдачи.
* **Результат:** Прототип обрабатывает тысячи позиций номенклатуры, сопоставляя их с тендерами по семантическому смыслу, а не просто по ключевым словам.

#### ✈️ Авиахакатон 2025 (МАИ / Т1)
**Трек:** «Системный взлёт».
* Спроектировал отказоустойчивую архитектуру для высоконагруженного сервиса в условиях жестких таймингов хакатона.

---

---

### 📈 Моя активность на GitHub

<p align="center">
  <img height="180" src="https://github-readme-stats-eight-theta.vercel.app/api?username=Alezovv&show_icons=true&theme=radical&include_all_commits=true&count_private=true" />
  <img height="180" src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=Alezovv&layout=compact&theme=radical&langs_count=8" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Alezovv&theme=radical" />
</p>

---


### 📫 Контакты
* **Telegram:** [@alezovv](https://t.me/alezovv)
* **Email:** alezovv2523@gmail.com
